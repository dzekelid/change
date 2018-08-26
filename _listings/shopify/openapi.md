---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
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
---