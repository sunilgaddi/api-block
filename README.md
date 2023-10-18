# api-block

% swagger-parameter in="path" name="id" type="String" %
Description
{% endswagger-parameter %}

{% swagger-parameter in="query" name="id" type="String" required="true" %}
Description
{% endswagger-parameter %}

{% swagger-parameter in="header" name="id" type="String" %}
Description
{% endswagger-parameter %}

{% swagger-parameter in="cookie" name="id" type="String" %}
Description
{% endswagger-parameter %}

{% swagger-parameter in="body" name="id" type="String" %}
Description
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="Description" %}
```javascript
{
    // good Response
}
```
{% endswagger-response %}
jnjnjnjn,,,

{% swagger-parameter in="path" name="id" type="String" %} Description {% endswagger-parameter %}

{% swagger-parameter in="query" name="id" type="String" required="true" %} Description {% endswagger-parameter %}

{% swagger-parameter in="header" name="id" type="String" %} Description {% endswagger-parameter %}

{% swagger-parameter in="cookie" name="id" type="String" %} Description {% endswagger-parameter %}

{% swagger-parameter in="body" name="id" type="String" %} Description {% endswagger-parameter %}

{% swagger-response status="200: OK" description="Description" %}

{
    // good Response
}
{% endswagger-response %} 

<details>

<summary>Expandable title</summary>

Expandable content

</details>


### Get Resource

- **URL**: `/api/resource/{id}`
- **Method**: GET
- **Description**: Retrieve a resource by its ID.

#### Request

No request body is required.

#### Parameters

| Parameter | Type    | Description        |
| --------- | ------- | ------------------ |
| id        | Integer | The ID of the resource to retrieve. |

#### Response

- **200 OK**:

```json
{
  "id": 1,
  "name": "Resource Name",
  "description": "A sample resource"
}
404 Not Found:
json
Copy code
{
  "message": "Resource not found"
}
Create Resource
URL: /api/resource
Method: POST
Description: Create a new resource.
Request
Headers:

Content-Type: application/json
Parameters
Parameter	Type	Description
name	String	The name of the resource.
description	String	A description of the resource.
Response
201 Created:
json
Copy code
{
  "id": 2,
  "name": "New Resource",
  "description": "A newly created resource"
}
400 Bad Request:
json
Copy code
{
  "message": "Validation failed"
}
Update Resource
URL: /api/resource/{id}
Method: PUT
Description: Update an existing resource.
Request
Headers:

Content-Type: application/json
Parameters
Parameter	Type	Description
id	Integer	The ID of the resource to update.
name	String	The updated name of the resource.
description	String	The updated description of the resource.
Response
200 OK:
json
Copy code
{
  "id": 2,
  "name": "Updated Resource",
  "description": "An updated resource"
}
404 Not Found:
json
Copy code
{
  "message": "Resource not found"
}
Delete Resource
URL: /api/resource/{id}
Method: DELETE
Description: Delete a resource by its ID.
Request
No request body is required.

Parameters
Parameter	Type	Description
id	Integer	The ID of the resource to delete.
Response
204 No Content:
No content is returned on success.

404 Not Found:
json
Copy code
{
  "message": "Resource not found"
}
Error Codes
400 Bad Request: The request is invalid.
401 Unauthorized: Authentication failed.
404 Not Found: The requested resource was not found.
500 Internal Server Error: An unexpected error occurred.
Rate Limits
Requests are limited to 100 per minute per API key.
Versioning
The API is currently at version 1.

This is a basic template for documenting an API using OpenAPI in Markdown format for GitBook. You can customize and expand this template to suit your specific API's needs and requirements.





