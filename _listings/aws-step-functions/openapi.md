swagger: "2.0"
x-collection-name: AWS Step Functions
x-complete: 1
info:
  title: AWS Step Functions API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StartExecution:
    get:
      summary: Start Execution
      description: Starts a state machine execution.
      operationId: startExecution
      x-api-path-slug: actionstartexecution-get
      parameters:
      - in: query
        name: input
        description: The JSON input data for the execution
        type: string
      - in: query
        name: name
        description: The name of the execution
        type: string
      - in: query
        name: stateMachineArn
        description: The Amazon Resource Name (ARN) of the state machine to execute
        type: string
      responses:
        200:
          description: OK
      tags:
      - State Machine