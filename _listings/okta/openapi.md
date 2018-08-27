swagger: "2.0"
x-collection-name: Okta
x-complete: 1
info:
  title: Users (Okta API)
  description: the-okta-user-apidocsapirestusers-html-provides-operations-to-manage-users-in-your-organization-
  version: 1.0.0
host: example.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{userId}/credentials/change_password:
    post:
      summary: Change Password
      description: Change password.
      operationId: postUsersUserCredentialsChangePassword
      x-api-path-slug: usersuseridcredentialschange-password-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Change
      - Password
  /users/{userId}/credentials/change_recovery_question:
    post:
      summary: Change Recovery Question
      description: Change recovery question.
      operationId: postUsersUserCredentialsChangeRecoveryQuestion
      x-api-path-slug: usersuseridcredentialschange-recovery-question-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Change
      - Recovery
      - Question