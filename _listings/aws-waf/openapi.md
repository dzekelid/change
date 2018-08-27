swagger: "2.0"
x-collection-name: AWS WAF
x-complete: 1
info:
  title: AWS WAF API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetChangeToken:
    get:
      summary: Get Change Token
      description: 'Service: AWS WAFWhen you want to create, update, or delete AWS
        WAF objects, get a change token and include the change token in the create,
        update, or delete request.'
      operationId: getChangeToken
      x-api-path-slug: actiongetchangetoken-get
      parameters:
      - in: query
        name: ChangeToken
        description: The ChangeToken that you used in the request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Change Token
  /?Action=GetChangeTokenStatus:
    get:
      summary: Get Change Token Status
      description: 'Service: AWS WAFReturns the status of a ChangeToken that you got
        by calling.'
      operationId: getChangeTokenStatus
      x-api-path-slug: actiongetchangetokenstatus-get
      parameters:
      - in: query
        name: ChangeToken
        description: The change token for which you want to get the status
        type: string
      responses:
        200:
          description: OK
      tags:
      - Change Token