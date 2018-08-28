swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 1
info:
  title: AWS EC2 Systems Manager API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetInventory:
    get:
      summary: Get Inventory
      description: Query inventory information.
      operationId: getInventory
      x-api-path-slug: actiongetinventory-get
      parameters:
      - in: query
        name: Filters
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: ResultAttributes
        description: The list of inventory item types to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Inventory
  /?Action=GetParameterHistory:
    get:
      summary: Get Parameter History
      description: Query a list of all parameters used by the AWS account.
      operationId: getParameterHistory
      x-api-path-slug: actiongetparameterhistory-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: Name
        description: The name of a parameter you want to query
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: WithDecryption
        description: Return decrypted values for secure string parameters
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameter
      - History