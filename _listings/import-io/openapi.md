swagger: "2.0"
x-collection-name: Import.io
x-complete: 1
info:
  title: import.io
  version: "1.0"
host: schedule.import.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /extractor/{extractorId}/start:
    post:
      summary: Post Extractor Extractorid Start
      description: Launch a crawl from an extractor that a user owns..
      operationId: postExtractorExtractorStart
      x-api-path-slug: extractorextractoridstart-post
      parameters:
      - in: path
        name: extractorId
        description: the id of the extractor to start crawling with
      - in: query
        name: loginSessionId
        description: The loginSessionId required for authenticated extractors
      responses:
        200:
          description: OK
      tags:
      - Extractor
      - ExtractorId
      - Start