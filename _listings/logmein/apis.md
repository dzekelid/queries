---
name: LogMeIn
x-slug: logmein
description: LogMeIn, Inc. is a provider of software as a service and cloud-based
  remote connectivity services for collaboration, IT management and customer engagement,
  founded in 2003 and based in Boston, Massachusetts.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
x-kinRank: "7"
x-alexaRank: "7271"
tags: Queries
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/logmein/apis.md
specificationVersion: "0.14"
apis:
- name: GoToAssist Remote Support - Get Tickets
  x-api-slug: get
  description: "Retrieves a query-able set of tickets for a specific partner system.\n\n
    \                                                        \nRequest Parameters\n
    \                         \n    field      data type      description    \n    userToken
    \     string      The token identifying and authenticating the user in the partner
    system that this object is being created on behalf of this user.    \n\n\nQuery
    Parameters (* Optional)\n\n    field      data type      description    \n    q
    *      string      A query string used to search for objects in the partner system.
    (It is up to the partner system to determine how the query string is matched.
    Match against fields like: ticket title, ticket body, requester name, ticket ID,
    ticket comments, tags, etc. Ideally the matching should be performed using a \u2018contains\u2019
    type operation and in a case-insensitive way.)                                         \n
    \   limit *      integer      The maximum number of records to be fetched. Default
    value is 10. Suggested value is less than or equal to 10 for optimal performance.
    \                                        \n    offset *      number      Zero
    based offset for the first record to return. Default value is 0."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2A/rest/v1
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/logmein/get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/logmein/get-openapi.md
- name: GoToAssist Remote Support - Get Tickets
  x-api-slug: get
  description: "Retrieves a query-able set of tickets for a specific partner system.\n\n
    \                                                        \nRequest Parameters\n
    \                         \n    field      data type      description    \n    userToken
    \     string      The token identifying and authenticating the user in the partner
    system that this object is being created on behalf of this user.    \n\n\nQuery
    Parameters (* Optional)\n\n    field      data type      description    \n    q
    *      string      A query string used to search for objects in the partner system.
    (It is up to the partner system to determine how the query string is matched.
    Match against fields like: ticket title, ticket body, requester name, ticket ID,
    ticket comments, tags, etc. Ideally the matching should be performed using a \u2018contains\u2019
    type operation and in a case-insensitive way.)                                         \n
    \   limit *      integer      The maximum number of records to be fetched. Default
    value is 10. Suggested value is less than or equal to 10 for optimal performance.
    \                                        \n    offset *      number      Zero
    based offset for the first record to return. Default value is 0."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2A/rest/v1
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/logmein/get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/logmein/get-openapi.md
x-common:
- type: x-github
  url: https://github.com/logmein
- type: x-openapi
  url: https://www.getpostman.com/collections/94ad52bdc3d954bad52a
- type: x-postman-collection
  url: https://www.getpostman.com/collections/00bf4391e993c3afa7b7
- type: x-postman-collection
  url: https://www.getpostman.com/collections/c35d614484f21e581775
- type: x-postman-collection
  url: https://www.getpostman.com/collections/9c6e067461f45f7faa6b
- type: x-postman-collection
  url: https://drive.google.com/open?id=16WZlBkS1i8cWSfZ3mMKOwlNP-qsE7AWy
- type: x-postman-collection
  url: https://drive.google.com/file/d/1vI11FNCKpv6WJ_70hoqPNMmPAkASiOU_/view?usp=sharing
- type: x-website
  url: http://www.LogMeInInc.com
- type: x-api-gallery
  url: http://loginradius.api.gallery.streamdata.io
- type: x-api-stack
  url: http://logmein.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/logmein
- type: x-developer
  url: https://goto-developer.logmeininc.com/
- type: x-documentation
  url: https://goto-developer.logmeininc.com/apis/apis-overview
- type: x-faq
  url: https://goto-developer.logmeininc.com/faq-page
- type: x-support
  url: https://goto-developer.logmeininc.com/api-support-request-template
- type: x-twitter
  url: https://twitter.com/LogMeIn
- type: x-website
  url: https://www.logmeininc.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---