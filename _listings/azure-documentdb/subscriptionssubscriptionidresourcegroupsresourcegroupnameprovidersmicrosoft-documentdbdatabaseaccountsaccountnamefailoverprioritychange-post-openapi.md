---
swagger: "2.0"
x-collection-name: Azure DocumentDB
x-complete: 0
info:
  title: Azure DocumentDB API Database Accounts Failover Priority Change
  description: Changes the failover priority for the Azure DocumentDB database account.
    A failover priority of 0 indicates a write region. The maximum value for a failover
    priority = (total number of regions - 1). Failover priority values must be unique
    for each of the regions in which the database account exists.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts/{accountName}/failoverPriorityChange
  : post:
      summary: Database Accounts Failover Priority Change
      description: Changes the failover priority for the Azure DocumentDB database
        account. A failover priority of 0 indicates a write region. The maximum value
        for a failover priority = (total number of regions - 1). Failover priority
        values must be unique for each of the regions in which the database account
        exists.
      operationId: DatabaseAccounts_FailoverPriorityChange
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-documentdbdatabaseaccountsaccountnamefailoverprioritychange-post
      parameters:
      - in: body
        name: failoverParameters
        description: The new failover policies for the database account
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Database
      - Accounts
      - Failover
      - Priority
      - Change
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