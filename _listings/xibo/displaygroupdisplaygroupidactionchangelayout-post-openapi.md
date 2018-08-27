---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: 'Xibo API Action: Change Layout'
  description: Send the change layout action to this DisplayGroup
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /displaygroup/{displayGroupId}/action/changeLayout:
    post:
      summary: 'Action: Change Layout'
      description: Send the change layout action to this DisplayGroup
      operationId: displayGroupActionChangeLayout
      x-api-path-slug: displaygroupdisplaygroupidactionchangelayout-post
      parameters:
      - in: formData
        name: changeMode
        description: Whether to queue or replace with this action
      - in: path
        name: displayGroupId
        description: The Display Group Id
      - in: formData
        name: downloadRequired
        description: Flag indicating whether the player should perform a collect before
          playing the Layout
      - in: formData
        name: duration
        description: The duration in seconds for this Layout change to remain in effect
      - in: formData
        name: layoutId
        description: The Layout Id
      responses:
        200:
          description: OK
      tags:
      - 'Action:'
      - Change
      - Layout
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