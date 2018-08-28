---
swagger: "2.0"
x-collection-name: AWS EC2 Container Service
x-complete: 0
info:
  title: Amazon EC2 Container Service API Start Task
  version: 1.0.0
  description: |-
    Starts a new task from the specified task definition on the specified container
                instance or instances.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RunTask:
    get:
      summary: Run Task
      description: Starts a new task using the specified task definition.
      operationId: runTask
      x-api-path-slug: actionruntask-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          on which to run your task
        type: string
      - in: query
        name: count
        description: The number of instantiations of the specified task to place on
          your            cluster
        type: string
      - in: query
        name: group
        description: The name of the task group to associate with the task
        type: string
      - in: query
        name: overrides
        description: A list of container overrides in JSON format that specify the
          name of a container            in the specified task definition and the
          overrides it should receive
        type: string
      - in: query
        name: placementConstraints
        description: An array of placement constraint objects to use for the task
        type: string
      - in: query
        name: placementStrategy
        description: The placement strategy objects to use for the task
        type: string
      - in: query
        name: startedBy
        description: An optional tag specified when a task is started
        type: string
      - in: query
        name: taskDefinition
        description: The family and revision (family:revision) or            full
          Amazon Resource Name (ARN) of the task definition to run
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=StartTask:
    get:
      summary: Start Task
      description: |-
        Starts a new task from the specified task definition on the specified container
                    instance or instances.
      operationId: startTask
      x-api-path-slug: actionstarttask-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          on which to start your task
        type: string
      - in: query
        name: containerInstances
        description: The container instance IDs or full Amazon Resource Name (ARN)
          entries for the container instances on            which you would like to
          place your task
        type: string
      - in: query
        name: group
        description: The name of the task group to associate with the task
        type: string
      - in: query
        name: overrides
        description: A list of container overrides in JSON format that specify the
          name of a container            in the specified task definition and the
          overrides it should receive
        type: string
      - in: query
        name: startedBy
        description: An optional tag specified when a task is started
        type: string
      - in: query
        name: taskDefinition
        description: The family and revision (family:revision) or            full
          Amazon Resource Name (ARN) of the task definition to start
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
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