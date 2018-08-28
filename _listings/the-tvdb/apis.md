---
name: The TVDB
x-slug: the-tvdb
description: TheTVDB.com is a community driven database of television shows. All content
  and images on the site have been contributed by the sites users; the site uses moderated
  editing to maintain its own standards. The database schema and website are open
  source under the GNU General Public License.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
x-kinRank: "7"
x-alexaRank: "0"
tags: Queries
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/apis.md
specificationVersion: "0.14"
apis:
- name: The TVDB API v2 - Get Series Episodes Query
  x-api-slug: seriesidepisodesquery-get
  description: This route allows the user to query against episodes for the given
    series. The response is a paginated array of episode records that have been filtered
    down to basic information.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/seriesidepisodesquery-get-openapi.md
- name: The TVDB API v2 - Get Series Episodes Query Params
  x-api-slug: seriesidepisodesqueryparams-get
  description: Returns the allowed query keys for the `/series/{id}/episodes/query`
    route
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/seriesidepisodesqueryparams-get-openapi.md
- name: The TVDB API v2 - Get Series Images Query
  x-api-slug: seriesidimagesquery-get
  description: Query images for the given series ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/seriesidimagesquery-get-openapi.md
- name: The TVDB API v2 - Get Series Images Query Params
  x-api-slug: seriesidimagesqueryparams-get
  description: Returns the allowed query keys for the `/series/{id}/images/query`
    route. Contains a parameter record for each unique `keyType`, listing values that
    will return results.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/seriesidimagesqueryparams-get-openapi.md
- name: The TVDB API v2 - Get Updated Query
  x-api-slug: updatedquery-get
  description: |-
    Returns an array of series that have changed in a maximum of one week blocks since the provided `fromTime`.


    The user may specify a `toTime` to grab results for less than a week. Any timespan larger than a week will be reduced down to one week automatically.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/updatedquery-get-openapi.md
- name: The TVDB API v2 - Get Updated Query Params
  x-api-slug: updatedqueryparams-get
  description: Returns an array of valid query keys for the `/updated/query/params`
    route.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/updatedqueryparams-get-openapi.md
- name: The TVDB API v2 - Get User Ratings Query
  x-api-slug: userratingsquery-get
  description: Returns an array of ratings for a given user that match the query.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/userratingsquery-get-openapi.md
- name: The TVDB API v2 - Get User Ratings Query Params
  x-api-slug: userratingsqueryparams-get
  description: Returns a list of query params for use in the `/user/ratings/query`
    route.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/userratingsqueryparams-get-openapi.md
- name: The TVDB API v2 - Get Series Episodes Query
  x-api-slug: seriesidepisodesquery-get
  description: This route allows the user to query against episodes for the given
    series. The response is a paginated array of episode records that have been filtered
    down to basic information.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/seriesidepisodesquery-get-openapi.md
- name: The TVDB API v2 - Get Series Episodes Query Params
  x-api-slug: seriesidepisodesqueryparams-get
  description: Returns the allowed query keys for the `/series/{id}/episodes/query`
    route
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/seriesidepisodesqueryparams-get-openapi.md
- name: The TVDB API v2 - Get Series Images Query
  x-api-slug: seriesidimagesquery-get
  description: Query images for the given series ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/seriesidimagesquery-get-openapi.md
- name: The TVDB API v2 - Get Series Images Query Params
  x-api-slug: seriesidimagesqueryparams-get
  description: Returns the allowed query keys for the `/series/{id}/images/query`
    route. Contains a parameter record for each unique `keyType`, listing values that
    will return results.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/seriesidimagesqueryparams-get-openapi.md
- name: The TVDB API v2 - Get Updated Query
  x-api-slug: updatedquery-get
  description: |-
    Returns an array of series that have changed in a maximum of one week blocks since the provided `fromTime`.


    The user may specify a `toTime` to grab results for less than a week. Any timespan larger than a week will be reduced down to one week automatically.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/updatedquery-get-openapi.md
- name: The TVDB API v2 - Get Updated Query Params
  x-api-slug: updatedqueryparams-get
  description: Returns an array of valid query keys for the `/updated/query/params`
    route.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/updatedqueryparams-get-openapi.md
- name: The TVDB API v2 - Get User Ratings Query
  x-api-slug: userratingsquery-get
  description: Returns an array of ratings for a given user that match the query.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/userratingsquery-get-openapi.md
- name: The TVDB API v2 - Get User Ratings Query Params
  x-api-slug: userratingsqueryparams-get
  description: Returns a list of query params for use in the `/user/ratings/query`
    route.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/userratingsqueryparams-get-openapi.md
- name: The TVDB API v2 - Get User Ratings Query Params
  x-api-slug: userratingsqueryparams-get
  description: Returns a list of query params for use in the `/user/ratings/query`
    route.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/userratingsqueryparams-get-openapi.md
- name: The TVDB API v2 - Get User Ratings Query
  x-api-slug: userratingsquery-get
  description: Returns an array of ratings for a given user that match the query.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/userratingsquery-get-openapi.md
- name: The TVDB API v2 - Get Updated Query Params
  x-api-slug: updatedqueryparams-get
  description: Returns an array of valid query keys for the `/updated/query/params`
    route.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/updatedqueryparams-get-openapi.md
- name: The TVDB API v2 - Get Updated Query
  x-api-slug: updatedquery-get
  description: |-
    Returns an array of series that have changed in a maximum of one week blocks since the provided `fromTime`.


    The user may specify a `toTime` to grab results for less than a week. Any timespan larger than a week will be reduced down to one week automatically.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/updatedquery-get-openapi.md
- name: The TVDB API v2 - Get Series Images Query Params
  x-api-slug: seriesidimagesqueryparams-get
  description: Returns the allowed query keys for the `/series/{id}/images/query`
    route. Contains a parameter record for each unique `keyType`, listing values that
    will return results.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/seriesidimagesqueryparams-get-openapi.md
- name: The TVDB API v2 - Get Series Images Query
  x-api-slug: seriesidimagesquery-get
  description: Query images for the given series ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/seriesidimagesquery-get-openapi.md
- name: The TVDB API v2 - Get Series Episodes Query Params
  x-api-slug: seriesidepisodesqueryparams-get
  description: Returns the allowed query keys for the `/series/{id}/episodes/query`
    route
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/seriesidepisodesqueryparams-get-openapi.md
- name: The TVDB API v2 - Get Series Episodes Query
  x-api-slug: seriesidepisodesquery-get
  description: This route allows the user to query against episodes for the given
    series. The response is a paginated array of episode records that have been filtered
    down to basic information.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/the-tvdb/seriesidepisodesquery-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://the.open.movie.database.api.gallery.streamdata.io
- type: x-api-stack
  url: http://the.tvdb.stack.network
- type: x-documentation
  url: https://api.thetvdb.com/swagger
- type: x-website
  url: http://thetvdb.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---