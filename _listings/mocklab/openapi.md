---
swagger: "2.0"
x-collection-name: MockLab
x-complete: 1
info:
  title: WireMock
  version: 1.0.0
basePath: /__admin
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /recordings/start:
    post:
      summary: Post Recordings Start
      description: Start recording stub mappings
      operationId: postRecordingsStart
      x-api-path-slug: recordingsstart-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Recordings
      - Start
---