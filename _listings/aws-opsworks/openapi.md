swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 1
info:
  title: AWS OpsWorks API
  version: 1.0.0
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