# Manitoba Skating Rinks API

Get a list of current skating rink locations within a specified kilometer radius of your choosing. Information for each skating rink includes: the name, the address, the postal code, and the phone number. Data is available exclusively in JSON.

# List of endpoints with parameters

## Endpoints
`http://www.skatingrink.com/location`
* Returns a list of skating rink locations that match the given parameters (see below).

## Parameters
| Name        | Type        | Description   |
| :---        |    :----:   |          :--- |
| Radius      | float       | Required. List of skating rink will be returned within this radius     |
| Size        | float       | Optional. Only specific size of skating rink will be returned          |
| Opened      | boolean     | Optional. Only opened skating rink will be returned if it is 'True'    |

# Description of resources - formatted as JSON

A List of available rinks in the radius are listed and each have 4 outputed resources which are: \
_Name_: A **String** containing the name of the rink. \
_Adress_: A **String** containing the address of the rink. \
_Postal_: A **String** containing the postal code of the rink. \
_Phone_: An **Integer** containing the phone number of the manager of the rink.

# Sample request with sample response


  

  

## Example

**Request**

    Get:  https://api.manitobaskatingrinks.org/info/1.0/getskatingrink?lat=42.103&lon=44.111&radius=20

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
      "lat": 51.2344,
      "long": 44.242,
      "rad": 12
    }
   ]

