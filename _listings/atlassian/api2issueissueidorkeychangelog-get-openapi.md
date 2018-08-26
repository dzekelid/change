---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get change logs
  description: Returns a [paginated](#pagination) list of all updates of an issue,
    sorted by date, starting from the oldest.
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/issue/{issueIdOrKey}/changelog:
    get:
      summary: Get change logs
      description: Returns a [paginated](#pagination) list of all updates of an issue,
        sorted by date, starting from the oldest.
      operationId: com.atlassian.jira.rest.v2.issue.IssueChangelogResource.getChangeLogs_get
      x-api-path-slug: api2issueissueidorkeychangelog-get
      parameters:
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue
      - in: query
        name: maxResults
        description: Maximum number of items to return per page
      - in: query
        name: startAt
        description: Page offset, ie
      responses:
        200:
          description: OK
      tags:
      - Change
      - Logs
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