swagger: "2.0"
x-collection-name: AWS WorkSpaces
x-complete: 1
info:
  title: AWS WorkSpaces Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StartWorkspaces:
    get:
      summary: Start Workspaces
      description: Starts the specified WorkSpaces.
      operationId: startWorkspaces
      x-api-path-slug: actionstartworkspaces-get
      parameters:
      - in: query
        name: StartWorkspaceRequests
        description: The requests
        type: string
      responses:
        200:
          description: OK
      tags:
      - Workspaces