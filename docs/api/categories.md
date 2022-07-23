# Categories
Categories can be reach through the URL `https://your-site-url/api/categories`.

## Retrieve all Categories
URL: `https://your-site-url/api/categories`  
Method: `GET`  
Response data:
```JSON
{
    "data": [
    {
        "id": 1,
        "name": "server",
        "label": "Server",
        "visible_in_navigation": 1,
        "parent_category": 0,
        "attributes": [
           "1",
           "2",
           "4"
        ],
        "icon": "fa fa-search",
        "sort_order": 10,
        "created_at": {
           "date": "2018-11-25 17:28:41.000000",
           "timezone_type": 3,
           "timezone": "UTC"
        },
        "updated_at": {
           "date": "2018-11-25 17:28:41.000000",
           "timezone_type": 3,
           "timezone": "UTC"
        }
        },
    .....
    ]
}
```

## Retrieve a Category
URL: `https://your-site-url/api/categories/{categoryid}`  
Method: `GET`  
Response data:
```JSON
{
    "data": {
        "id": 1,
        "name": "server",
        "label": "Server",
        "visible_in_navigation": 1,
        "parent_category": 0,
        "attributes": [
            "1",
            "2",
            "4"
        ],
        "icon": "fa fa-search",
        "sort_order": 10,
        "created_at": {
            "date": "2018-11-25 17:28:41.000000",
            "timezone_type": 3,
            "timezone": "UTC"
        },
        "updated_at": {
            "date": "2018-11-25 17:28:41.000000",
            "timezone_type": 3,
            "timezone": "UTC"
        }
    }
}
```

## Create a Category
URL: `https://your-site-url/api/categories`  
Method: `POST`  
Request body:
```JSON
{
    "name": "router",
    "label": "Router",
    "visible_in_navigation": 1,
    "parent_category": 0,
    "attributes": [
        "1",
        "2",
        "4"
    ],
    "icon": "fa fa-user",
    "sort_order": 10
}
```

Response body: see "Retrieve a Category"

## Update a Category
URL: `https://your-site-url/api/categories/{categoryid}`  
Method: `PUT`  
Request body:
```JSON
{
    "name": "router",
    "label": "Router",
    "visible_in_navigation": 1,
    "parent_category": 0,
    "attributes": [
        "1",
        "2",
        "4"
    ],
    "icon": "fa fa-user",
    "sort_order": 10
}
```

Response data: see "Retrieve a Category"

## Delete a Category
Not yet implemented.