---
swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 0
info:
  title: AWS OpsWorks API Start Instance
  version: 1.0.0
  description: Starts a specified instance.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StartInstance:
    get:
      summary: Start Instance
      description: Starts a specified instance.
      operationId: startInstance
      x-api-path-slug: actionstartinstance-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Start
      - Instance
  /?Action=StartStack:
    get:
      summary: Start Stack
      description: Starts a stack's instances.
      operationId: startStack
      x-api-path-slug: actionstartstack-get
      parameters:
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Start
      - Stack
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