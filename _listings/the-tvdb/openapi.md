swagger: "2.0"
x-collection-name: The TVDB
x-complete: 1
info:
  title: The TVDB API v2
  description: api-v2-targets-v1-functionality-with-a-few-minor-additions--the-api-is-accessible-via-httpsapi-thetvdb-com-and-provides-the-following-rest-endpoints-in-json-format-how-to-use-this-api-documentationyou-may-browse-the-api-routes-without-authentication-but-if-you-wish-to-send-requests-to-the-api-and-see-response-data-then-you-must-authenticate-1--obtain-a-jwt-token-by-posting--to-the-login-route-in-the-authentication-section-with-your-api-key-and-credentials-1--paste-the-jwt-token-from-the-response-into-the-jwt-token-field-at-the-top-of-the-page-and-click-the-add-token-button-you-will-now-be-able-to-use-the-remaining-routes-to-send-requests-to-the-api-and-get-a-response-language-selectionlanguage-selection-is-done-via-the-acceptlanguage-header--at-the-moment-you-may-only-pass-one-language-abbreviation-in-the-header-at-a-time--valid-language-abbreviations-can-be-found-at-the-languages-route--authenticationauthentication-to-use-the-api-is-similar-to-the-howto-section-above--users-must-post-to-the-login-route-with-their-api-key-and-credentials-in-the-following-format-in-order-to-obtain-a-jwt-token-apikeyapikeyusernameusernameuserkeyuserkeynote-that-the-username-and-key-are-only-required-for-the-user-routes--the-users-key-is-labled-account-identifier-in-the-account-section-of-the-main-site-the-token-is-then-used-in-all-subsequent-requests-by-providing-it-in-the-authorization-header--the-header-will-look-like-authorization-bearer-yourjwttoken--currently-the-token-expires-after-24-hours--you-can-get-the-refresh-token-route-to-extend-that-expiration-date-versioningyou-may-request-a-different-version-of-the-api-by-including-an-accept-header-in-your-request-with-the-following-format-acceptapplicationvnd-thetvdb-vversion--this-documentation-automatically-uses-the-version-seen-at-the-top-and-bottom-of-the-page-
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