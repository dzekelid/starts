---
swagger: "2.0"
x-collection-name: VMWare
x-complete: 0
info:
  title: VMWare vRealize Operations Start an adapter instance
  description: |-
    Replace the UUID with the ID of the adapter instance you want to start
    This can be retrieved using Get Adapter Instances
  version: 1.0.0
host: example.com
basePath: /suite-api/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/resources/{epopsMonitorResourceId}/monitoringstate/start:
    put:
      summary: Start Monitoring a Resource
      description: 'TODO: Add Description'
      operationId: ApiResourcesMonitoringstateStartByEpopsMonitorResourceIdPut
      x-api-path-slug: apiresourcesepopsmonitorresourceidmonitoringstatestart-put
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: epopsMonitorResourceId
      responses:
        200:
          description: OK
      tags:
      - Resources
      - EpopsMonitorResourceId
      - Monitoringstate
      - Start
  /api/adapters/617d20fd-536a-4bea-9f5e-4c01dd845ddc/monitoringstate/start:
    put:
      summary: Start an adapter instance
      description: |-
        Replace the UUID with the ID of the adapter instance you want to start
        This can be retrieved using Get Adapter Instances
      operationId: ApiAdapters617d20fd536a4bea9f5e4c01dd845ddcMonitoringstateStartPut
      x-api-path-slug: apiadapters617d20fd536a4bea9f5e4c01dd845ddcmonitoringstatestart-put
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Adapters
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