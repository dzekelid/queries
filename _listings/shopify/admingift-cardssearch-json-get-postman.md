{
  "info": {
    "name": "Shopify Get all gift cards that matches the query",
    "_postman_id": "050a5b7b-289f-49f1-8f2e-7971ebc035f2",
    "description": "Get all gift cards that matches the query.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "6939783c-2924-4f1b-b492-77d30516b032",
          "name": "getAdminGiftCards61466894.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/gift_cards/61466894.json",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
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
            "description": "Show a specific gift card's details."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5137e26-9ff2-4093-b1b3-435116b50e99"
            }
          ]
        },
        {
          "id": "b74a701a-e3e3-4f4b-befd-fb1eb4337ada",
          "name": "getAdminGiftCardsCount.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/gift_cards/count.json",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
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
            "description": "Retrieve a count of all gift cards."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "151c11bc-b1db-48a5-83ef-7a6e4f477399"
            }
          ]
        },
        {
          "id": "ebbe83d6-3b8a-47c6-9816-e294b90e1c59",
          "name": "getAdminGiftCards.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/gift_cards.json",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
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
            "description": "Get a list of all gift cards."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8af1dc63-681e-4587-ba57-31d1ad61d825"
            }
          ]
        },
        {
          "id": "392b273f-5a5f-40eb-899f-a467569e5b83",
          "name": "getAdminGiftCardsSearch.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/gift_cards/search.json?query=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
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
            "description": "Get all gift cards that matches the query."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e717e025-f7cf-474c-92f3-01c107118876"
            }
          ]
        }
      ]
    }
  ]
}