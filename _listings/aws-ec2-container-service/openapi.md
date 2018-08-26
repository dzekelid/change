---
swagger: "2.0"
x-collection-name: AWS EC2 Container Service
x-complete: 1
info:
  title: AWS EC2 Container Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=SubmitContainerStateChange:
    get:
      summary: Submit Container State Change
      description: This action is only used by the Amazon EC2 Container Service agent,
        and it is not intended for use outside of the agent.
      operationId: submitContainerStateChange
      x-api-path-slug: actionsubmitcontainerstatechange-get
      responses:
        200:
          description: OK
      tags:
      - Container State Change
  /?Action=SubmitTaskStateChange:
    get:
      summary: Submit Task State Change
      description: This action is only used by the Amazon EC2 Container Service agent,
        and it is not intended for use outside of the agent.
      operationId: submitTaskStateChange
      x-api-path-slug: actionsubmittaskstatechange-get
      responses:
        200:
          description: OK
      tags:
      - Task State Change
---