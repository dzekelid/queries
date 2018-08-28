{
  "info": {
    "name": "Google Fusion Tables API Execute SQL Statement",
    "_postman_id": "b56bf0f4-9588-4dab-84a4-f8b8d79c85e9",
    "description": "Executes a SQL statement which can be any of \n- SELECT\n- SHOW\n- DESCRIBE",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Query",
      "item": [
        {
          "id": "e5112919-6071-403e-a617-a0a454c4e0bf",
          "name": "fusiontables.query.sqlGet",
          "request": {
            "url": "http://www.googleapis.com/fusiontables/v2/query?hdrs=%7B%7D&sql=%7B%7D&typed=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Executes a SQL statement which can be any of \n- SELECT\n- SHOW\n- DESCRIBE"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a78705d-7608-4a06-9278-9c40c6a4b7db"
            }
          ]
        }
      ]
    }
  ]
}