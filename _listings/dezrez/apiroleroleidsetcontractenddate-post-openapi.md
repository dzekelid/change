---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Change the branch of a role
  version: 1.0.0
  description: Change the branch of a role.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/document/setprivacy:
    put:
      summary: Sets the document privacy for an existing document.  This is used to
        change a document from being publicly accessible to being private, and vice
        versa.
      description: Sets the document privacy for an existing document.  this is used
        to change a document from being publicly accessible to being private, and
        vice versa..
      operationId: Document_SetDocumentPrivacyBysetDocumentPrivacyCommand
      x-api-path-slug: apidocumentsetprivacy-put
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: setDocumentPrivacyCommand
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Document
      - Privacyan
      - Existing
      - Document
      - ""
      - ""
      - This
      - Is
      - Used
      - To
      - Change
      - Document
      - From
      - Being
      - Publicly
      - Accessible
      - To
      - Being
      - Private
      - ""
      - Vice
      - Versa
  /api/documentgeneration/renamelettertemplate/{id}:
    post:
      summary: Rename a letter template and change the description
      description: Rename a letter template and change the description.
      operationId: DocumentGeneration_UpdateLetterTemplateByidByrenameDataContract
      x-api-path-slug: apidocumentgenerationrenamelettertemplateid-post
      parameters:
      - in: path
        name: id
        description: Document Id for the template
      - in: body
        name: renameDataContract
        description: The letter template
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Rename
      - Letter
      - Template
      - Change
      - Description
  /api/progression/lettings/setestimatedmoveindate:
    put:
      summary: Change the estimated move in date for the tenancy.
      description: Change the estimated move in date for the tenancy..
      operationId: LettingsProgression_SetEstimatedMoveInDateBydataContract
      x-api-path-slug: apiprogressionlettingssetestimatedmoveindate-put
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Change
      - Estimated
      - Move
      - In
      - Datethe
      - Tenancy
  /api/receipt/payment/{id}/setexportstatus:
    post:
      summary: Change status export status of payment
      description: Change status export status of payment.
      operationId: Receipt_SetPaymentExportStatusByidBystatusDataContract
      x-api-path-slug: apireceiptpaymentidsetexportstatus-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: statusDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Change
      - Status
      - Export
      - Status
      - Of
      - Payment
  /api/role/{id}/changeteam:
    put:
      summary: Change the owining team of a Role
      description: Change the owining team of a role.
      operationId: Role_ChangeTeamByidByteamId
      x-api-path-slug: apiroleidchangeteam-put
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: teamId
      responses:
        200:
          description: OK
      tags:
      - Change
      - Owining
      - Team
      - Of
      - Role
  /api/role/{id}/changebranch:
    post:
      summary: Change the branch of a role
      description: Change the branch of a role.
      operationId: Role_ChangeBranchByidBybranchId
      x-api-path-slug: apiroleidchangebranch-post
      parameters:
      - in: query
        name: branchId
        description: Id of Branch
      - in: path
        name: id
        description: Id of Role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Change
      - Branch
      - Of
      - Role
  /api/role/{roleId}/setcontractenddate:
    post:
      summary: Change the branch of a role
      description: Change the branch of a role.
      operationId: Role_SetContractEndDateByroleIdByendDateDatContact
      x-api-path-slug: apiroleroleidsetcontractenddate-post
      parameters:
      - in: body
        name: endDateDatContact
        description: Id of Branch
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
        description: The role id
      responses:
        200:
          description: OK
      tags:
      - Change
      - Branch
      - Of
      - Role
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