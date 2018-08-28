{
  "info": {
    "name": "Google Fusion Tables API Execute Fusion Table SQL Statement",
    "_postman_id": "48851640-ecc1-4f19-8b1e-8e5cf9cef089",
    "description": "Executes a Fusion Tables SQL statement, which can be any of \n- SELECT\n- INSERT\n- UPDATE\n- DELETE\n- SHOW\n- DESCRIBE\n- CREATE statement.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Query",
      "item": [
        {
          "id": "c7ac3a95-82d9-4598-991a-9461d38cb18c",
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
              "id": "cc1a77cc-d43d-4eff-a75d-5b53b13f0b0e"
            }
          ]
        },
        {
          "id": "23acb6ba-5502-48fb-854d-9626e76df43c",
          "name": "fusiontables.query.sql",
          "request": {
            "url": "http://www.googleapis.com/fusiontables/v2/query?hdrs=%7B%7D&sql=%7B%7D&typed=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Executes a Fusion Tables SQL statement, which can be any of \n- SELECT\n- INSERT\n- UPDATE\n- DELETE\n- SHOW\n- DESCRIBE\n- CREATE statement."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4393dd9-0ef4-486f-be6c-48507f9dfc0d"
            }
          ]
        }
      ]
    }
  ]
}