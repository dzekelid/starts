---
swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 1
info:
  title: AWS Lightsale API
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
      description: Starts a specific Amazon Lightsail instance from a stopped state.
      operationId: startInstance
      x-api-path-slug: actionstartinstance-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance (a virtual private server) to start
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
---