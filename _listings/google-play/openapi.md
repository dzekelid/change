---
swagger: "2.0"
x-collection-name: Google Play
x-complete: 1
info:
  title: Google Play
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{packageName}/edits/{editId}:commit:
    post:
      summary: Commit Changes
      description: Commits/applies the changes made in this edit back to the app.
      operationId: androidpublisher.edits.commit
      x-api-path-slug: packagenameeditseditidcommit-post
      parameters:
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Change
  /{packageName}/edits/{editId}:validate:
    post:
      summary: Validate Changes
      description: Checks that the edit can be successfully committed. The edit's
        changes are not applied to the live app.
      operationId: androidpublisher.edits.validate
      x-api-path-slug: packagenameeditseditidvalidate-post
      parameters:
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Change
---