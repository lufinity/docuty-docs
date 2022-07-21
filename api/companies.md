# Companies

- ###### Table of Contents
- [Retrieve all Companies](#retrieve-all-companies)
- [Retrieve an Item](#retrieve-an-item)
- [Create a Company](#create-a-company)
- [Update a Company](#update-a-company)
- [Delete a Company](#delete-a-company)

Companies is one of the most straight forward models to work with. They can be reach through the URL `https://your-site-url/api/companies`.

<a name="retrieve-all-companies"></a>
## Retrieve all Companies

URL: `https://your-site-url/api/companies`  
Method: `GET`  
Response data:
```JSON
{
    "data": [
    {
        "id": {id},
        "name": {name},
        "active": {active},
        "regnr": {regnr},
        "street": {street},
        "zipcode": {zipcode},
        "city": {city},
        "phone": {phone},
        "email": {email},
        "webpage": {webpage},
        "country": {country},
        "created_at": dateTime,
        "updated_at": dateTime
    },
    .....
    ]
}
```

<a name="retrieve-an-item"></a>
## Retrieve an Item

URL: `https://your-site-url/api/companies/{companyid}`  
Method: `GET`  
Response data:
```JSON
{
    "data": {
        "id": {id},
        "name": {name},
        "active": {active},
        "regnr": {regnr},
        "street": {street},
        "zipcode": {zipcode},
        "city": {city},
        "phone": {phone},
        "email": {email},
        "webpage": {webpage},
        "country": {country},
        "created_at": dateTime,
        "updated_at": dateTime
    }
}
```

<a name="create-a-company"></a>
## Create a Company

URL: `https://your-site-url/api/companies`  
Method: `POST`  
Request body:
```JSON
{
    "name": "name",
    "active": 0/1,
    "regnr": "12345678",
    "streep": "Some street",
    "city": "some city",
    "phone": "07123456789",
    "email": "exmple@domain.se",
    "webpage": "https://example.se",
    "country": "Sweden"
}
```

Response body: see "Retrieve all Companies"

<a name="update-a-company"></a>
## Update a Company

URL: `https://your-site-url/api/companies/{companyid}`  
Method: `PUT`  
Request body:
```JSON
{
    "name": "name",
    "active": 0/1,
    "regnr": "12345678",
    "streep": "Some street",
    "city": "some city",
    "phone": "07123456789",
    "email": "exmple@domain.se",
    "webpage": "https://example.se",
    "country": "Sweden"
}
```

Response data: see "Retrieve all Companies"

<a name="delete-a-company"></a>
## Delete a Company

Not yet implemented.