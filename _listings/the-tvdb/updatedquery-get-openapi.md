---
swagger: "2.0"
x-collection-name: The TVDB
x-complete: 0
info:
  title: The TVDB Get Updated Query
  description: |-
    Returns an array of series that have changed in a maximum of one week blocks since the provided `fromTime`.


    The user may specify a `toTime` to grab results for less than a week. Any timespan larger than a week will be reduced down to one week automatically.
  version: 2.1.2
host: api-dev.thetvdb.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /series/{id}/episodes/query:
    get:
      summary: Get Series Episodes Query
      description: This route allows the user to query against episodes for the given
        series. The response is a paginated array of episode records that have been
        filtered down to basic information.
      operationId: series.id.episodes.query.get
      x-api-path-slug: seriesidepisodesquery-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Series
      - Episodes
      - Query
  /series/{id}/episodes/query/params:
    get:
      summary: Get Series Episodes Query Params
      description: Returns the allowed query keys for the `/series/{id}/episodes/query`
        route
      operationId: series.id.episodes.query.params.get
      x-api-path-slug: seriesidepisodesqueryparams-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Series
      - Episodes
      - Query
      - Params
  /series/{id}/images/query:
    get:
      summary: Get Series Images Query
      description: Query images for the given series ID.
      operationId: series.id.images.query.get
      x-api-path-slug: seriesidimagesquery-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Series
      - Images
      - Query
  /series/{id}/images/query/params:
    get:
      summary: Get Series Images Query Params
      description: Returns the allowed query keys for the `/series/{id}/images/query`
        route. Contains a parameter record for each unique `keyType`, listing values
        that will return results.
      operationId: series.id.images.query.params.get
      x-api-path-slug: seriesidimagesqueryparams-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Series
      - Images
      - Query
      - Params
  /updated/query:
    get:
      summary: Get Updated Query
      description: |-
        Returns an array of series that have changed in a maximum of one week blocks since the provided `fromTime`.


        The user may specify a `toTime` to grab results for less than a week. Any timespan larger than a week will be reduced down to one week automatically.
      operationId: updated.query.get
      x-api-path-slug: updatedquery-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Updated
      - Query
  /updated/query/params:
    get:
      summary: Get Updated Query Params
      description: Returns an array of valid query keys for the `/updated/query/params`
        route.
      operationId: updated.query.params.get
      x-api-path-slug: updatedqueryparams-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - Updated
      - Query
      - Params
  /user/ratings/query:
    get:
      summary: Get User Ratings Query
      description: Returns an array of ratings for a given user that match the query.
      operationId: user.ratings.query.get
      x-api-path-slug: userratingsquery-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Ratings
      - Query
  /user/ratings/query/params:
    get:
      summary: Get User Ratings Query Params
      description: Returns a list of query params for use in the `/user/ratings/query`
        route.
      operationId: user.ratings.query.params.get
      x-api-path-slug: userratingsqueryparams-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Ratings
      - Query
      - Params
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