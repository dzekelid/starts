---
swagger: "2.0"
x-collection-name: Import.io
x-complete: 0
info:
  title: import.io Post Extractor Extractorid Start
  version: "1.0"
  description: Launch a crawl from an extractor that a user owns..
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