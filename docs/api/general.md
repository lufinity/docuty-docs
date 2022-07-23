# General
To date the only possible API functions is to view, create, edit and delete companies, attributes, categories and entities. More functions will be added in future releases. All requests must include an access token in the header which is received by Code Null like so:  
```php
Headers: Authorization = Bearer [Access token]
```

All data in request body as well as response must be in JSON-format. Also, there are no restriction in the API. So the API-user can't have restricted permissions for certain companies, categories or attributes. This is to be implemented in later versions.