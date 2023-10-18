```yaml
openapi: 3.0.0
info:
  title: Sample API
  version: 1.0.0
paths:
  /users:
    get:
      summary: Get a list of users
      responses:
        200:
          description: A list of users
          content:
            application/json:
              example:
                - id: 1
                  name: John
                - id: 2
                  name: Jane
```
