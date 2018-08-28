{
  "info": {
    "name": "Framesocket Query Media",
    "_postman_id": "cc04e135-dac6-4b88-8f82-d04ac8b8aa5e",
    "description": "Query Media",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Media",
      "item": [
        {
          "id": "77dcacc4-ed81-46a7-9b5a-226b61903ee0",
          "name": "getMediaActivate.php",
          "request": {
            "url": "http://www.framesocket.com/api/media/activate.php?customid=%7B%7D&hash=%7B%7D&key=%7B%7D&secret=%7B%7D&sig=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Activate Media"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a8d7d4b-36a2-4862-a0b9-cdad996abfb2"
            }
          ]
        },
        {
          "id": "9597062c-7f02-4a7f-b997-c6630934d9b7",
          "name": "getMediaDeactivate.php",
          "request": {
            "url": "http://www.framesocket.com/api/media/deactivate.php?customid=%7B%7D&hash=%7B%7D&key=%7B%7D&secret=%7B%7D&sig=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deactive Media"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac4073b8-2c98-4b5d-8c1a-f0b5fddbc812"
            }
          ]
        },
        {
          "id": "0bd6c503-315c-4892-ae00-0362b352673b",
          "name": "getMediaImages.php",
          "request": {
            "url": "http://www.framesocket.com/api/media/images.php?customid=%7B%7D&hash=%7B%7D&key=%7B%7D&secret=%7B%7D&sig=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Query Images"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c42c10f9-bd61-4ebf-b869-1ad5917416da"
            }
          ]
        },
        {
          "id": "e70347c9-529b-40f1-9629-2f9fdec82bbb",
          "name": "getMediaQuery.php",
          "request": {
            "url": "http://www.framesocket.com/api/media/query.php?andkeywords=%7B%7D&andtitlewords=%7B%7D&customid=%7B%7D&hash=%7B%7D&key=%7B%7D&limit=%7B%7D&orkeywords=%7B%7D&ortitlewords=%7B%7D&secret=%7B%7D&sig=%7B%7D&sort=%7B%7D&status=%7B%7D&type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Query Media"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0f71f3ab-05d8-420d-b2a3-616929e7a9b1"
            }
          ]
        }
      ]
    }
  ]
}