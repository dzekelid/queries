---
swagger: "2.0"
x-collection-name: Europeana
x-complete: 0
info:
  title: Europeana translate a term to different languages
  description: Translate a term to different languages.
  termsOfService: http://www.europeana.eu/portal/en/rights.html
  contact:
    name: http://labs.europeana.eu/api
  version: 1.0.0
host: www.europeana.eu
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /translateQuery.json:
    get:
      summary: translate a term to different languages
      description: Translate a term to different languages.
      operationId: translateQueryUsingGET
      x-api-path-slug: translatequery-json-get
      parameters:
      - in: query
        name: callback
        description: callback
      - in: query
        name: languageCodes
        description: languageCodes
      - in: query
        name: profile
        description: profile
      - in: query
        name: term
        description: term
      - in: query
        name: wskey
        description: wskey
      responses:
        200:
          description: OK
      tags:
      - Translations
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