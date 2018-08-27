---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Change an existing liquid template's value
  description: Change an existing liquid template's value.
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/themes/110163843/assets.json:
    put:
      summary: Change an existing liquid template's value
      description: Change an existing liquid template's value.
      operationId: putAdminThemes110163843Assets.json
      x-api-path-slug: adminthemes110163843assets-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Change
      - Existing
      - Liquid
      - Templates
      - Value
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