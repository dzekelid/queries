swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/city/{query}:
    get:
      summary: Get City Query
      description: Get city query.
      operationId: getApiV1CityQuery
      x-api-path-slug: apiv1cityquery-get
      parameters:
      - in: path
        name: query
      responses:
        200:
          description: OK
      tags:
      - City
      - Query
  /api/v1/country/{query}:
    get:
      summary: Get Country Query
      description: Get country query.
      operationId: getApiV1CountryQuery
      x-api-path-slug: apiv1countryquery-get
      parameters:
      - in: path
        name: query
      responses:
        200:
          description: OK
      tags:
      - Country
      - Query
  /api/v1/genre/{query}:
    get:
      summary: Get Genre Query
      description: Get genre query.
      operationId: getApiV1GenreQuery
      x-api-path-slug: apiv1genrequery-get
      parameters:
      - in: path
        name: query
      responses:
        200:
          description: OK
      tags:
      - Genre
      - Query
  /api/v1/gigme/genre/{query}:
    get:
      summary: Get Gigme Genre Query
      description: Get gigme genre query.
      operationId: getApiV1GigmeGenreQuery
      x-api-path-slug: apiv1gigmegenrequery-get
      parameters:
      - in: path
        name: query
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Genre
      - Query
  /api/v1/place/{cityId}/search/{query}:
    get:
      summary: Get Place Cityid Search Query
      description: Get place cityid search query.
      operationId: getApiV1PlaceCitySearchQuery
      x-api-path-slug: apiv1placecityidsearchquery-get
      parameters:
      - in: path
        name: cityId
      - in: path
        name: query
      responses:
        200:
          description: OK
      tags:
      - Place
      - Cityid
      - Search
      - Query