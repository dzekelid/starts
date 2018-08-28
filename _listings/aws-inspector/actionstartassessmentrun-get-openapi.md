---
swagger: "2.0"
x-collection-name: AWS Inspector
x-complete: 0
info:
  title: AWS Inspector API Start Assessment Run
  version: 1.0.0
  description: Starts the assessment run specified by the ARN of the assessment template.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StartAssessmentRun:
    get:
      summary: Start Assessment Run
      description: Starts the assessment run specified by the ARN of the assessment
        template.
      operationId: startAssessmentRun
      x-api-path-slug: actionstartassessmentrun-get
      parameters:
      - in: query
        name: assessmentRunName
        description: You can specify the name for the assessment run
        type: string
      - in: query
        name: assessmentTemplateArn
        description: The ARN of the assessment template of the assessment run that
          you want to         start
        type: string
      responses:
        200:
          description: OK
      tags:
      - Assessment Runs
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