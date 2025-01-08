# springdoc-nullable_fields-issue

Open Api Specification generated with SpringDoc v2.8.1 (nullable: true is absent):

```json
{
  "openapi": "3.1.0",
  "info": {
    "title": "OpenAPI definition",
    "version": "v0"
  },
  "servers": [
    {
      "url": "http://localhost:8080",
      "description": "Generated server url"
    }
  ],
  "paths": {
    "/cat": {
      "get": {
        "tags": [
          "basic-controller"
        ],
        "summary": "get",
        "description": "Provides an animal.",
        "operationId": "get",
        "parameters": [
          {
            "name": "cat",
            "in": "query",
            "required": true,
            "schema": {
              "$ref": "#/components/schemas/Cat"
            }
          }
        ],
        "responses": {
          "200": {
            "description": "OK",
            "content": {
              "*/*": {
                "schema": {
                  "type": "string"
                }
              }
            }
          }
        }
      }
    }
  },
  "components": {
    "schemas": {
      "Cat": {
        "type": "object",
        "description": "Represents a Cat class.",
        "properties": {
          "name": {
            "type": "string",
            "description": "The name."
          }
        }
      }
    }
  }
}
```

Open Api Specification generated with SpringDoc v2.7.0 (nullable: true is present):

```json
{
  "openapi": "3.0.1",
  "info": {
    "title": "OpenAPI definition",
    "version": "v0"
  },
  "servers": [
    {
      "url": "http://localhost:8080",
      "description": "Generated server url"
    }
  ],
  "paths": {
    "/cat": {
      "get": {
        "tags": [
          "basic-controller"
        ],
        "summary": "get",
        "description": "Provides an animal.",
        "operationId": "get",
        "parameters": [
          {
            "name": "cat",
            "in": "query",
            "required": true,
            "schema": {
              "$ref": "#/components/schemas/Cat"
            }
          }
        ],
        "responses": {
          "200": {
            "description": "OK",
            "content": {
              "*/*": {
                "schema": {
                  "type": "string"
                }
              }
            }
          }
        }
      }
    }
  },
  "components": {
    "schemas": {
      "Cat": {
        "type": "object",
        "description": "Represents a Cat class."
        "properties": {
          "name": {
            "type": "string",
            "description": "The name.",
            "nullable": true
          }
        },
      }
    }
  }
}
```