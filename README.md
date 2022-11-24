# Manitoba Skating Rinks API

Get a list of current skating rink locations within a specified kilometer radius of your choosing. Information for each skating rink includes: the name, the address, the postal code, and the phone number. Data is available exclusively in JSON.

# List of endpoints with parameters

# Description of resources - formatted as JSON

# Sample request with sample response


  

## Example

**Request**

    Get:  https://api.manitobaskatingrinks.org/info/1.0/getskatingrink?lat=42.103&lon=44.111&radius=20

**Response:**

    [
     {
      "name": "Manitoba Skating, 
      "address": "2080 pembina hwy, Winnipeg, MB",
      "postal": "R3T2G9", 
      "phone": "2041232222"
    }, 
     { "name": "Dakota Skating Rig",
     'address": "61 clayton Drive, Winnipeg, MB", 
     "phone": "2041232222" 
     }
    ]


