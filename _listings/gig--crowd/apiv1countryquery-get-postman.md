{
  "info": {
    "name": "GIGANDCROWD Get Country Query",
    "_postman_id": "dcb080fd-a4b5-4fd4-a43b-066ecdadc9de",
    "description": "Get country query.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Message",
      "item": [
        {
          "id": "6d76589f-acce-47e0-af94-d40f6d294091",
          "name": "getApiV1MessageCountUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/message/count/:userId"
              ],
              "variable": [
                {
                  "id": "userId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get message count userid."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc59f7d8-9f97-44ea-9b08-2d7ac9a611b0"
            }
          ]
        }
      ]
    },
    {
      "name": "Country",
      "item": [
        {
          "id": "432dc1b1-1cdc-4527-a1da-f18f25254358",
          "name": "getApiV1CountryQuery",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/country/:query"
              ],
              "variable": [
                {
                  "id": "query",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get country query."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66e23615-b107-46c4-af6d-43880b5202c2"
            }
          ]
        }
      ]
    }
  ]
}