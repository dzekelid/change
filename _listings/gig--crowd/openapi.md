swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/gigme/password/change:
    post:
      summary: Post Gigme Password Change
      description: Post gigme password change.
      operationId: postApiV1GigmePasswordChange
      x-api-path-slug: apiv1gigmepasswordchange-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Password
      - Change
  /api/v1/password/change:
    post:
      summary: Post Password Change
      description: Post password change.
      operationId: postApiV1PasswordChange
      x-api-path-slug: apiv1passwordchange-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Password
      - Change