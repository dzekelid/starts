---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 1
info:
  title: AWS EC2 Systems Manager API
  version: 1.0.0
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
---