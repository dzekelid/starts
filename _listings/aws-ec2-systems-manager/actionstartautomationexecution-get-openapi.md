---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 0
info:
  title: Amazon EC2 Systems Manager API Start Automation Execution
  version: 1.0.0
  description: Initiates execution of an Automation document.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StartAutomationExecution:
    get:
      summary: Start Automation Execution
      description: Initiates execution of an Automation document.
      operationId: startAutomationExecution
      x-api-path-slug: actionstartautomationexecution-get
      parameters:
      - in: query
        name: DocumentName
        description: The name of the Automation document to use for this execution
        type: string
      - in: query
        name: DocumentVersion
        description: The version of the Automation document to use for this execution
        type: string
      - in: query
        name: Parameters
        description: A key-value map of execution parameters, which match the declared
          parameters in the Automation document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Start
      - Automation
      - Execution
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