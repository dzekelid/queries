{
  "info": {
    "name": "GIGANDCROWD Get Gigme Genre Query",
    "_postman_id": "403c027a-9e9f-4e2d-b251-49d21bb8000d",
    "description": "Get gigme genre query.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "City",
      "item": [
        {
          "id": "5b2d9ba5-a974-4f59-a6ef-df3afcb777dc",
          "name": "getApiV1CityQuery",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/city/:query"
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
            "description": "Get city query."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "697b21a4-b45a-461e-9fe3-94ab3026a964"
            }
          ]
        }
      ]
    },
    {
      "name": "Country",
      "item": [
        {
          "id": "58c2e574-d1ed-4cd1-8a7b-d530e4a8fd64",
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
              "id": "bd1b3af4-f53e-4003-a73b-70cff6bacf2b"
            }
          ]
        }
      ]
    },
    {
      "name": "Genre",
      "item": [
        {
          "id": "b9c0c4ed-4322-4036-8a6f-1fcd45f97136",
          "name": "getApiV1GenreQuery",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/genre/:query"
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
            "description": "Get genre query."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42319c56-5f90-4d20-8cd9-e20abf39c6ca"
            }
          ]
        }
      ]
    },
    {
      "name": "Gigme",
      "item": [
        {
          "id": "e83ee381-86ac-4d32-9a09-13c3b7b9a181",
          "name": "getApiV1GigmeGenreQuery",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/gigme/genre/:query"
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
            "description": "Get gigme genre query."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00415b65-346e-4c29-a55a-96d124ff39ac"
            }
          ]
        }
      ]
    },
    {
      "name": "Place",
      "item": [
        {
          "id": "ae2dd104-8490-4d6c-aa50-b16dba54d69f",
          "name": "getApiV1PlaceCitySearchQuery",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/place/:cityId/search/:query"
              ],
              "variable": [
                {
                  "id": "cityId",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Get place cityid search query."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f6ce91b9-b9f1-4ea7-9403-107b427bbd62"
            }
          ]
        }
      ]
    }
  ]
}