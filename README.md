# Manitoba Skating Rinks API

Get a list of current skating rink locations within a specified kilometer radius of your choosing. Information for each skating rink includes: the name, the address, the postal code, and the phone number. Data is available exclusively in JSON.

# List of endpoints with parameters

## Endpoints
`/getSkatingRink`
* Returns a list of skating rink locations that match the given parameters (see below).

## Parameters
| Name        | Type        | Description   |
| :---        |    :----:   |          :--- |
| lat         | number       | Required. Latitude of the location in Manitoba where you want to look for skating  rinks |         |
| long        | number       | Required. Longitude of the location in Manitoba where you want to look for skating  rinks |
| Radius      | integer      | Required. Radius of the search area |

# Description of resources - formatted as JSON

A List of available rinks in the radius are listed and each have 4 outputed resources which are: \


    [  
    { 
    "id": An  **integer**  identifying the rinks uniquely.
    "name": A  **string**  containing the name of the rink.  
    "address": A  **string**  containing the address of the rink.  
    "postal": A  string  containing the postal code of the rink.  
    "phone": An  **integer**  containing the phone number of the manager of the rink.  
    "params": An **object** that contains information about the paramenters passed to the API.  
    }  
    ]


# Sample request with sample response


  

  

## Example

**Request**

    Get:  https://api.manitobaskatingrinks.org/getSkatingRink?lat=42.103&lon=44.111&radius=20

**Response:**

    [
     {
      "id":1,
      "name": "Manitoba Skating, 
      "address": "2080 pembina hwy, Winnipeg, MB",
      "postal": "R3T2G9", 
      "phone": "2041232222"
     }, 
     {
     "id":2,
     "name": "Dakota Skating Rig",
     "address": "61 clayton Drive, Winnipeg, MB",
     "postal": "R2M1G1", 
     "phone": "2041232222" 
     },
     "params": {
      "lat": 42.103,
      "long": 44.111,
      "rad": 12
    }
   ]

