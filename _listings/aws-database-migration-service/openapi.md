---
swagger: "2.0"
x-collection-name: AWS Database Migration Service
x-complete: 1
info:
  title: AWS Database Migration Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StartReplicationTask:
    get:
      summary: Start Replication Task
      description: Starts the replication task.
      operationId: startReplicationTask
      x-api-path-slug: actionstartreplicationtask-get
      parameters:
      - in: query
        name: CdcStartTime
        description: The start time for the Change Data Capture (CDC) operation
        type: string
      - in: query
        name: ReplicationTaskArn
        description: The Amazon Resource Number (ARN) of the replication task to be
          started
        type: string
      - in: query
        name: StartReplicationTaskType
        description: The type of replication task
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Tasks
---