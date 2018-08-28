{
  "info": {
    "name": "Amazon DynamoDB API Query",
    "_postman_id": "e35e58c0-6822-476d-a722-459e154290ee",
    "description": "A Query operation uses the primary key of a table or a secondary index\n            to directly access items from that table or index.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Batch Items",
      "item": [
        {
          "id": "48835a00-ea99-4337-be36-556bcb1cd517",
          "name": "batchGetItem",
          "request": {
            "url": "http://example.com/api/?Action=BatchGetItem?RequestItems=RequestItems&ReturnConsumedCapacity=ReturnConsumedCapacity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The BatchGetItem operation returns the attributes of one or more items from one or\n      more tables."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "32c1271e-a5ca-44eb-a506-80dc9d7fd739"
            }
          ]
        },
        {
          "id": "b51ba880-9db6-4a73-9adb-f9b4d41532d1",
          "name": "batchWriteItem",
          "request": {
            "url": "http://example.com/api/?Action=BatchWriteItem?RequestItems=RequestItems&ReturnConsumedCapacity=ReturnConsumedCapacity&ReturnItemCollectionMetrics=ReturnItemCollectionMetrics",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The BatchWriteItem operation puts or deletes multiple items in one or more tables."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "203ff071-f833-471f-93f2-dd96f183a6ed"
            }
          ]
        }
      ]
    },
    {
      "name": "Tables",
      "item": [
        {
          "id": "a767779b-25f6-4dc3-a055-ef79e49877da",
          "name": "createTable",
          "request": {
            "url": "http://example.com/api/?Action=CreateTable?AttributeDefinitions=AttributeDefinitions&GlobalSecondaryIndexes=GlobalSecondaryIndexes&KeySchema=KeySchema&LocalSecondaryIndexes=LocalSecondaryIndexes&ProvisionedThroughput=ProvisionedThroughput&StreamSpecification=StreamSpecification&TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The CreateTable operation adds a new table to your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce9dfc2b-9f9a-4ae5-9f11-c91767ea496e"
            }
          ]
        },
        {
          "id": "3c0eda61-0e13-437f-9c66-d6108882ac44",
          "name": "deleteTable",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTable?TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The DeleteTable operation deletes a table and all of its items."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ff6f016-eb2d-4ff2-a48d-927bc6884597"
            }
          ]
        },
        {
          "id": "20da7854-14f7-435e-9916-577c9cb1ef7b",
          "name": "describeTable",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTable?TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the table, including the current status of the table, when it was created, the primary key schema, and any indexes on the table."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76c5738b-701f-4ca9-936a-13b7b3a3dcc4"
            }
          ]
        },
        {
          "id": "75e3a14a-e2ae-4015-b67e-ce797456073e",
          "name": "listTables",
          "request": {
            "url": "http://example.com/api/?Action=ListTables?ExclusiveStartTableName=ExclusiveStartTableName&Limit=Limit",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns an array of table names associated with the current account and endpoint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7cd046f1-a593-44f3-8202-0cd77e069ee8"
            }
          ]
        }
      ]
    },
    {
      "name": "Items",
      "item": [
        {
          "id": "8ddecb40-cec1-4c2a-8ae7-e0ef9aa22c20",
          "name": "deleteItem",
          "request": {
            "url": "http://example.com/api/?Action=DeleteItem?ConditionalOperator=ConditionalOperator&ConditionExpression=ConditionExpression&Expected=Expected&ExpressionAttributeNames=ExpressionAttributeNames&ExpressionAttributeValues=ExpressionAttributeValues&Key=Key&ReturnConsumedCapacity=ReturnConsumedCapacity&ReturnItemCollectionMetrics=ReturnItemCollectionMetrics&ReturnValues=ReturnValues&TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a single item in a table by primary key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83284aa6-fb86-4eeb-b2dd-841ed0615170"
            }
          ]
        },
        {
          "id": "1d35f7a7-d447-439f-a42b-81e7bf2f7a77",
          "name": "getItem",
          "request": {
            "url": "http://example.com/api/?Action=GetItem?AttributesToGet=AttributesToGet&ConsistentRead=ConsistentRead&ExpressionAttributeNames=ExpressionAttributeNames&Key=Key&ProjectionExpression=ProjectionExpression&ReturnConsumedCapacity=ReturnConsumedCapacity&TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The GetItem operation returns a set of attributes for the item with the given primary\n          key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c20fe93-3e53-4e49-8272-aab5177f0342"
            }
          ]
        },
        {
          "id": "a4dac121-89bb-4871-8a9c-3237a5f20bdd",
          "name": "putItem",
          "request": {
            "url": "http://example.com/api/?Action=PutItem?ConditionalOperator=ConditionalOperator&ConditionExpression=ConditionExpression&Expected=Expected&ExpressionAttributeNames=ExpressionAttributeNames&ExpressionAttributeValues=ExpressionAttributeValues&Item=Item&ReturnConsumedCapacity=ReturnConsumedCapacity&ReturnItemCollectionMetrics=ReturnItemCollectionMetrics&ReturnValues=ReturnValues&TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new item, or replaces an old item with a new item."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34faf1cc-e6f8-4834-a8bf-34824defd6de"
            }
          ]
        }
      ]
    },
    {
      "name": "Limits",
      "item": [
        {
          "id": "bf1b0e96-363e-4833-b9af-744ea8ea24ce",
          "name": "describeLimits",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLimits?AccountMaxReadCapacityUnits=AccountMaxReadCapacityUnits&AccountMaxWriteCapacityUnits=AccountMaxWriteCapacityUnits&TableMaxReadCapacityUnits=TableMaxReadCapacityUnits&TableMaxWriteCapacityUnits=TableMaxWriteCapacityUnits",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the current provisioned-capacity limits for your AWS account in a region, both for the region as a whole and for any one DynamoDB table that you create there."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53bfa539-9a7b-4284-9e07-4f84f0df9b2c"
            }
          ]
        }
      ]
    },
    {
      "name": "Query",
      "item": [
        {
          "id": "19c60291-b943-4416-a62e-60c0a5b65177",
          "name": "query",
          "request": {
            "url": "http://example.com/api/?Action=Query?AttributesToGet=AttributesToGet&ConditionalOperator=ConditionalOperator&ConsistentRead=ConsistentRead&ExclusiveStartKey=ExclusiveStartKey&ExpressionAttributeNames=ExpressionAttributeNames&ExpressionAttributeValues=ExpressionAttributeValues&FilterExpression=FilterExpression&IndexName=IndexName&KeyConditionExpression=KeyConditionExpression&KeyConditions=KeyConditions&Limit=Limit&ProjectionExpression=ProjectionExpression&QueryFilter=QueryFilter&ReturnConsumedCapacity=ReturnConsumedCapacity&ScanIndexForward=ScanIndexForward&Select=Select&TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A Query operation uses the primary key of a table or a secondary index\n            to directly access items from that table or index."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e016f364-3a5c-4324-8951-125e8a4b1f87"
            }
          ]
        }
      ]
    }
  ]
}