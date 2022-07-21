# Entities

- ###### Table of Contents
- [Retrieve all Entities](#retrieve-all-entities)
- [Retrieve an Entity](#retrieve-an-entity)
- [Create an Entity/Entities](#create-an-entity)
- [Update an Entity/Entities](#update-an-entity)
- [Delete an Entity](#delete-an-entity)

Category entities can be reach through the URL `https://your-site-url/api/category-entities`.

<a name="retrieve-all-entities"></a>
## Retrieve all Entities

URL: `https://your-site-url/api/category-entities`  
Method: `GET`  
Response data:
```JSON
{
    "data": {
        "id": 1,
        "category_id": 1,
        "company_id": 1,
        "attributes": [
            {
                "id": 1,
                "attribute_id": 1,
                "entity_id": 1,
                "value": "attribute value"
            },
            {
                "id": 2,
                "attribute_id": 4,
                "entity_id": 1,
                "value": "attribute value"
            }
        ],
        "created_at": {
            "date": "2018-11-25 17:59:49.000000",
            "timezone_type": 3,
            "timezone": "UTC"
        },
        "updated_at": {
            "date": "2018-11-25 17:59:49.000000",
            "timezone_type": 3,
            "timezone": "UTC"
        }
    },
    .....
    ]
}
```

<a name="retrieve-an-entity"></a>
## Retrieve an Entity

URL: `https://your-site-url/api/category-entities/{entityid}`  
Method: `GET`  
Response data:
```JSON
{
    "data": {
        "id": 1,
        "category_id": 1,
        "company_id": 1,
        "attributes": [
            {
                "id": 1,
                "attribute_id": 1,
                "entity_id": 1,
                "value": "attribute value"
            },
            {
                "id": 2,
                "attribute_id": 4,
                "entity_id": 1,
                "value": "attribute value"
            }
        ],
        "created_at": {
            "date": "2018-11-25 17:59:49.000000",
            "timezone_type": 3,
            "timezone": "UTC"
        },
        "updated_at": {
            "date": "2018-11-25 17:59:49.000000",
            "timezone_type": 3,
            "timezone": "UTC"
        }
    }
}
```

<a name="create-an-entity"></a>
## Create an Entity/Entities

URL: `https://your-site-url/api/category-entities`  
Method: `POST`  
Request body:
```JSON
[
    {
        "category_id": 3,
        "company_id": 3,
        "attributes": [
           {
    	       "attribute": 1/"atttribute name",
               "value": "attribute value"
            },
            {
               "attribute": 1/"atttribute name",
               "value": "attribute value"
            }
        ]
    }
]
```
Note that you post an array so it is possible to create multiple entities at once. 
If one creation fails, all will fail so if you get an error you need make the full request again to create all entities.

> {info.fa-info-circle} You can specify the attribute id or the name of the attribute.  
Text field attributes only accept a string and no HTML. The value will go though an htmlspecialchars_decode.

Response body: see "Retrieve an Entity"

<a name="update-an-entity"></a>
## Update or create an Entity/Entities

URL: `https://you-site-url/api/category-entities/{entityid}`  
Method: `PUT`  
Request body:
```JSON
[
    {
        "id": 1
        "category_id": 3,
        "company_id": 3,
        "attributes": [
           {
    	       "attribute": 1/"atttribute name",
               "value": "attribute value"
            },
            {
               "attribute": 1/"atttribute name",
               "value": "attribute value"
            }
        ]
    }
]
```
If "id" is omitted a new entity will be created.

Note that you post an array so it is possible to create multiple entities at once. 
If one creation fails, all will fail so if you get an error you need make the full request again to create all entities.

> {info.fa-info-circle} You can specify the attribute id or the name of the attribute.  
Text field attributes only accept a string and no HTML. The value will go though an htmlspecialchars_decode.

Response data: see "Retrieve an Entity"

<a name="delete-an-entity"></a>
## Delete an Entity

Not yet implemented.