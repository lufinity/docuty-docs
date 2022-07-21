# Attributes

- ###### Table of Contents
- [Retrieve all Attributes](#retrieve-all-attributes)
- [Retrieve an Attribute](#retrieve-an-Attribute)
- [Create an Attribute](#create-an-attribute)
- [Update an Attribute](#update-an-attribute)
- [Delete an Attribute](#delete-an-attribute)

Attributes can be reach through the URL `https://your-site-url/api/attributes`.

<a name="retrieve-all-attributes"></a>
## Retrieve all Attributes

URL: `https://your-site-url/api/attributes`  
Method: `GET`  
Response data:
```JSON
{
    "data": [
        {
            "id": 1,
            "type": "varchar",
            "name": "name",
            "label": "Name",
            "description": null,
            "visible_in_listing": 1,
            "visible_in_form": 0,
            "required": 1,
            "encrypted": 0,
            "hidden": 0,
            "input_mask": null
        },
        {
            "id": 2,
            "type": "text",
            "name": "description",
            "label": "Description",
            "description": null,
            "visible_in_listing": 0,
            "visible_in_form": 1,
            "required": 0,
            "encrypted": 0,
            "hidden": 0,
            "input_mask": null
        },
    .....
    ]
}
```

<a name="retrieve-an-Attribute"></a>
## Retrieve an Attribute

URL: `https://your-site-url/api/attributes/{attributeid}`  
Method: `GET`  
Response data:
```JSON
{
    "data": {
        "id": null,
        "type": null,
        "name": null,
        "label": null,
        "description": null,
        "visible_in_listing": null,
        "visible_in_form": null,
        "required": null,
        "encrypted": null,
        "hidden": null,
        "input_mask": null
    }
}
```

<a name="create-an-attribute"></a>
## Create an Attribute

URL: `https://your-site-url/api/attributes`  
Method: `POST`  
Request body:
```JSON
{
    "type": "varchar",
    "name": "new_attribute",
    "label": "New attribute",
    "description": null,
    "visible_in_listing": 1,
    "visible_in_form": 0,
    "required": 1,
    "encrypted": 0,
    "hidden": 0,
    "input_mask": null
}
```

Response body: see "Retrieve an Attribute"

<a name="update-an-attribute"></a>
## Update an Attribute

URL: `https://your-site-url/api/attributes/{attributeid}`  
Method: `PUT`  
Request body:
```JSON
{
    "type": "varchar",
    "name": "new_attribute",
    "label": "New attribute",
    "description": null,
    "visible_in_listing": 1,
    "visible_in_form": 0,
    "required": 1,
    "encrypted": 0,
    "hidden": 0,
    "input_mask": null
}
```

Response data: see "Retrieve an Attribute"

<a name="delete-an-attribute"></a>
## Delete an Attribute

Not yet implemented.