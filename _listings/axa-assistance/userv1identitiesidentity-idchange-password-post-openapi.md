---
swagger: "2.0"
x-collection-name: AXA Assistance
x-complete: 0
info:
  title: AXA Assistance Change identity password
  description: Change identity password
  version: 1.0.0
host: sandbox.api.axa-assistance.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/v1/identities/forgot_password/confirm:
    post:
      summary: Confirm identity password change
      description: Confirm identity password change
      operationId: postUserV1IdentitiesForgot_passwordConfirm
      x-api-path-slug: userv1identitiesforgot-passwordconfirm-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Confirm
      - identity
      - password
      - change
  /user/v1/identities/{identity_id}/change_password:
    post:
      summary: Change identity password
      description: Change identity password
      operationId: postUserV1IdentitiesIdentity_idChange_password
      x-api-path-slug: userv1identitiesidentity-idchange-password-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: identity_id
        description: ID of the identity
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Change
      - identity
      - password
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