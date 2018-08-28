{
  "info": {
    "name": "GIGANDCROWD Get Genre Query",
    "_postman_id": "be157cbf-36eb-45d2-a4a2-c6bedeb69b6e",
    "description": "Get genre query.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "City",
      "item": [
        {
          "id": "2c284ebc-ada9-4513-b938-e5d510925f3e",
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
              "id": "ebf4bed8-5b6e-4f41-9d00-71a568af32dd"
            }
          ]
        }
      ]
    },
    {
      "name": "Country",
      "item": [
        {
          "id": "0c13d9fb-7ce1-4056-a9e1-2f26d6a0772a",
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
              "id": "5471d360-cc57-491a-82a8-2b1d83f19b95"
            }
          ]
        }
      ]
    },
    {
      "name": "Genre",
      "item": [
        {
          "id": "89aad44f-43ea-4b40-aba9-d4107b77c96c",
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
              "id": "72a820bc-5d5c-400c-aa02-0cae944dfb50"
            }
          ]
        }
      ]
    },
    {
      "name": "Gigme",
      "item": [
        {
          "id": "1ddb5af2-77e2-44d5-904b-5e5ce86450af",
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
              "id": "d25ae54a-643a-4203-9072-95ba311b57f4"
            }
          ]
        }
      ]
    },
    {
      "name": "Place",
      "item": [
        {
          "id": "4e87b530-7d2d-4622-9f3d-21f49cecebb4",
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
              "id": "61745641-443d-459a-99f6-165bd17e5015"
            }
          ]
        }
      ]
    }
  ]
}