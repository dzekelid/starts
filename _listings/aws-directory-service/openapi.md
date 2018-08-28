swagger: "2.0"
x-collection-name: AWS Directory Service
x-complete: 1
info:
  title: AWS Directory Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StartSchemaExtension:
    get:
      summary: Start Schema Extension
      description: Applies a schema extension to a Microsoft AD directory.
      operationId: startSchemaExtension
      x-api-path-slug: actionstartschemaextension-get
      parameters:
      - in: query
        name: CreateSnapshotBeforeSchemaExtension
        description: If true, creates a snapshot of the directory before applying
          the schema extension
        type: string
      - in: query
        name: Description
        description: A description of the schema extension
        type: string
      - in: query
        name: DirectoryId
        description: The identifier of the directory for which the schema extension
          will be applied to
        type: string
      - in: query
        name: LdifContent
        description: The LDIF file represented as a string
        type: string
      responses:
        200:
          description: OK
      tags:
      - Schema Extension