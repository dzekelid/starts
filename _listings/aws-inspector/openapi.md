---
swagger: "2.0"
x-collection-name: AWS Inspector
x-complete: 1
info:
  title: AWS Inspector API
  version: 1.0.0
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
---