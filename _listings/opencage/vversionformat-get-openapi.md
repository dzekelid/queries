---
swagger: "2.0"
x-collection-name: OpenCage
x-complete: 0
info:
  title: OpenCage Geocode Query
  description: Geocode a query
  termsOfService: https://geocoder.opencagedata.com/terms
  contact:
    name: OpenCage Data Ltd
    url: https://geocoder.opencagedata.com/contact
  version: 1.0.0
host: api.opencagedata.com
basePath: v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v{version}/{format}:
    get:
      summary: Geocode Query
      description: Geocode a query
      operationId: vversion.format.get
      x-api-path-slug: vversionformat-get
      parameters:
      - in: query
        name: abbrv
        description: when true we attempt to abbreviate the formatted field in the
          response
      - in: query
        name: add_request
        description: if true the request is included in the response
      - in: query
        name: bounds
        description: four coordinate points forming the south-west and north-east
          corners of a bounding box (min long, min lat, max long, max lat)
      - in: query
        name: countrycode
        description: two letter code ISO 3166-1 Alpha 2 code to limit results to that
          country
      - in: path
        name: format
        description: format of the response
      - in: query
        name: jsonp
        description: wraps the returned JSON with a function name
      - in: query
        name: key
        description: an application key
      - in: query
        name: language
        description: 'an IETF format language code (ex: es or pt-BR)'
      - in: query
        name: limit
        description: maximum number of results to return
      - in: query
        name: min_confidence
        description: integer from 1-10
      - in: query
        name: no_annotations
        description: when true annotations are not added to results
      - in: query
        name: no_dedupe
        description: when true results are not deduplicated
      - in: query
        name: no_record
        description: when true query content is not logged
      - in: query
        name: pretty
        description: when true results are pretty printed
      - in: query
        name: q
        description: string or lat,lng to be geocoded
      - in: path
        name: version
        description: API version
      responses:
        200:
          description: OK
      tags:
      - Geo
      - Encoding
      - Query
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---