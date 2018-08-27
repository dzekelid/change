---
name: Azure DocumentDB
x-slug: azure-documentdb
description: Azure DocumentDB is a fully-managed NoSQL document database service that
  offers querying and transaction-processing over schema-free data, predictable and
  reliable performance, and rapid development.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-document-db-03-replicate.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Change
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/change/master/_listings/azure-documentdb/apis.md
specificationVersion: "0.14"
apis:
- name: DocumentDB - Database Accounts Failover Priority Change
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-documentdbdatabaseaccountsaccountnamefailoverprioritychange-post
  description: Changes the failover priority for the Azure DocumentDB database account.
    A failover priority of 0 indicates a write region. The maximum value for a failover
    priority = (total number of regions - 1). Failover priority values must be unique
    for each of the regions in which the database account exists.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-document-db-03-replicate.png
  humanURL: https://azure.microsoft.com/en-us/services/documentdb/
  baseURL: ://management.azure.com//
  tags: Microsoft, Documents, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/change/master/_listings/azure-documentdb/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-documentdbdatabaseaccountsaccountnamefailoverprioritychange-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://azure.dns.api.gallery.streamdata.io
- type: x-api-stack
  url: http://azure.documentdb.stack.network
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/documentdb/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/documentdb/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/documentdb/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/documentdb/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---