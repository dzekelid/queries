swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/gift_cards/search.json:
    get:
      summary: Get all gift cards that matches the query
      description: Get all gift cards that matches the query.
      operationId: getAdminGiftCardsSearch.json
      x-api-path-slug: admingift-cardssearch-json-get
      parameters:
      - in: header
        name: Content-Type
      - in: query
        name: query
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Gift
      - Cards
      - That
      - Matches
      - Query