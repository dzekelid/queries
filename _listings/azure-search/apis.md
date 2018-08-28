---
name: Azure Search
x-slug: azure-search
description: Azure Search is a fully-managed service for adding sophisticated search
  capabilities to web and mobile applications without the typical complexities of
  full-text search.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Queries
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/azure-search/apis.md
specificationVersion: "0.14"
apis:
- name: SearchManagementClient - Query Keys Create
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamecreatequerykeyname-post
  description: Generates a new query key for the specified Search service. You can
    create up to 50 query keys per service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com//
  tags: Search, Microsoft, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamecreatequerykeyname-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamecreatequerykeyname-post-openapi.md
- name: SearchManagementClient - Query Keys List By Search Service
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamelistquerykeys-get
  description: Returns the list of query API keys for the given Azure Search service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com//
  tags: Search, Microsoft, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamelistquerykeys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamelistquerykeys-get-openapi.md
- name: SearchManagementClient - Query Keys Delete
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamedeletequerykeykey-delete
  description: Deletes the specified query key. Unlike admin keys, query keys are
    not regenerated. The process for regenerating a query key is to delete and then
    recreate it.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com//
  tags: Search, Microsoft, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamedeletequerykeykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamedeletequerykeykey-delete-openapi.md
- name: SearchManagementClient - Query Keys Create
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamecreatequerykeyname-post
  description: Generates a new query key for the specified Search service. You can
    create up to 50 query keys per service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com//
  tags: Search, Microsoft, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamecreatequerykeyname-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamecreatequerykeyname-post-openapi.md
- name: SearchManagementClient - Query Keys List By Search Service
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamelistquerykeys-get
  description: Returns the list of query API keys for the given Azure Search service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com//
  tags: Search, Microsoft, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamelistquerykeys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamelistquerykeys-get-openapi.md
- name: SearchManagementClient - Query Keys Delete
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamedeletequerykeykey-delete
  description: Deletes the specified query key. Unlike admin keys, query keys are
    not regenerated. The process for regenerating a query key is to delete and then
    recreate it.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com//
  tags: Search, Microsoft, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamedeletequerykeykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamedeletequerykeykey-delete-openapi.md
- name: SearchManagementClient - Query Keys Delete
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamedeletequerykeykey-delete
  description: Deletes the specified query key. Unlike admin keys, query keys are
    not regenerated. The process for regenerating a query key is to delete and then
    recreate it.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com//
  tags: Search, Microsoft, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamedeletequerykeykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamedeletequerykeykey-delete-openapi.md
- name: SearchManagementClient - Query Keys List By Search Service
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamelistquerykeys-get
  description: Returns the list of query API keys for the given Azure Search service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com//
  tags: Search, Microsoft, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamelistquerykeys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamelistquerykeys-get-openapi.md
- name: SearchManagementClient - Query Keys Create
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamecreatequerykeyname-post
  description: Generates a new query key for the specified Search service. You can
    create up to 50 query keys per service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com//
  tags: Search, Microsoft, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamecreatequerykeyname-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queries/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamecreatequerykeyname-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://azure.scheduler.api.gallery.streamdata.io
- type: x-api-stack
  url: http://azure.search.stack.network
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/search/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/search/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/search/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/search/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---