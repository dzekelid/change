---
swagger: "2.0"
x-collection-name: Google Drive
x-complete: 0
info:
  title: Google Drive Get Start Page Token Changes
  description: Gets the starting pageToken for listing future changes.
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: v3
host: www.googleapis.com
basePath: /drive/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /changes:
    get:
      summary: Get Changes
      description: Lists the changes for a user or Team Drive.
      operationId: drive.changes.list
      x-api-path-slug: changes-get
      parameters:
      - in: query
        name: includeCorpusRemovals
        description: Whether changes should include the file resource if the file
          is still accessible by the user at the time of the request, even when a
          file was removed from the list of changes and there will be no further change
          entries for this file
      - in: query
        name: includeRemoved
        description: Whether to include changes indicating that items have been removed
          from the list of changes, for example by deletion or loss of access
      - in: query
        name: includeTeamDriveItems
        description: Whether Team Drive files or changes should be included in results
      - in: query
        name: pageSize
        description: The maximum number of changes to return per page
      - in: query
        name: pageToken
        description: The token for continuing a previous list request on the next
          page
      - in: query
        name: restrictToMyDrive
        description: Whether to restrict the results to changes inside the My Drive
          hierarchy
      - in: query
        name: spaces
        description: A comma-separated list of spaces to query within the user corpus
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      - in: query
        name: teamDriveId
        description: The Team Drive from which changes will be returned
      responses:
        200:
          description: OK
      tags:
      - Change
  /changes/startPageToken:
    get:
      summary: Get Start Page Token Changes
      description: Gets the starting pageToken for listing future changes.
      operationId: drive.changes.getStartPageToken
      x-api-path-slug: changesstartpagetoken-get
      parameters:
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      - in: query
        name: teamDriveId
        description: The ID of the Team Drive for which the starting pageToken for
          listing future changes from that Team Drive will be returned
      responses:
        200:
          description: OK
      tags:
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