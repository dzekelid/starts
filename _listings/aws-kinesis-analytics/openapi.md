swagger: "2.0"
x-collection-name: AWS Kinesis Analytics
x-complete: 1
info:
  title: AWS Kinesis Analytics API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StartApplication:
    get:
      summary: Start Application
      description: Starts the specified Amazon Kinesis Analytics application.
      operationId: startApplication
      x-api-path-slug: actionstartapplication-get
      parameters:
      - in: query
        name: ApplicationName
        description: Name of the application
        type: string
      - in: query
        name: InputConfigurations
        description: Identifies the specific input, by ID, that the application starts
          consuming
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications