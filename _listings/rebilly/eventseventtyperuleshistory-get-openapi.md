---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Retrieve the change history of the set of rules
  description: |-
    Retrieve the change history of the selected set of rules.
    The history is updated each time you change the rules.
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /authentication-options:
    put:
      summary: Change authentication options
      description: Change options
      operationId: authentication_options.put
      x-api-path-slug: authenticationoptions-put
      parameters:
      - in: body
        name: body
        description: Authentication Options resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Change
      - Authentication
      - Options
  /custom-events/{id}/rules/history:
    get:
      summary: Retrieve the change history of the set of rules for a custom event
      description: |-
        Retrieve the change history of the set of rules for the selected custom event.
        The history is updated each time you change the rules.
      operationId: retrieve-the-change-history-of-the-set-of-rules-for-the-selected-custom-event-the-history-is-updated
      x-api-path-slug: customeventsidruleshistory-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Change
      - History
      - Of
      - Set
      - Of
      - Rulesa
      - Custom
      - Event
  /custom-events/{id}/rules/history/{version}:
    get:
      summary: Retrieve the record from the change history of the set of rules for
        a custom event
      description: |-
        Retrieve the record from the change history of the set of rules for the selected custom event.
        A history record is created each time you change the rules.
      operationId: retrieve-the-record-from-the-change-history-of-the-set-of-rules-for-the-selected-custom-event-a-hist
      x-api-path-slug: customeventsidruleshistoryversion-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Record
      - From
      - Change
      - History
      - Of
      - Set
      - Of
      - Rulesa
      - Custom
      - Event
  /events/{eventType}/rules/history:
    get:
      summary: Retrieve the change history of the set of rules
      description: |-
        Retrieve the change history of the selected set of rules.
        The history is updated each time you change the rules.
      operationId: retrieve-the-change-history-of-the-selected-set-of-rules-the-history-is-updated-each-time-you-change
      x-api-path-slug: eventseventtyperuleshistory-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Change
      - History
      - Of
      - Set
      - Of
      - Rules
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