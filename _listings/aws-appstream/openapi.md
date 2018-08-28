swagger: "2.0"
x-collection-name: AWS AppStream
x-complete: 1
info:
  title: AWS AppStream 2.0 API
  description: amazon-appstream-2-0-is-a-fully-managed-secure-application-streaming-service-that-allows-you-to-stream-desktop-applications-from-aws-to-any-device-running-a-web-browser-without-rewriting-them--amazon-appstream-2-0-provides-users-instanton-access-to-the-applications-they-need-and-a-responsive-fluid-user-experience-on-the-device-of-their-choice-
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StartFleet:
    get:
      summary: Start Fleet
      description: Starts a fleet.
      operationId: StartFleet
      x-api-path-slug: actionstartfleet-get
      parameters:
      - in: query
        name: Name
        description: The name of the fleet to start
        type: string
      responses:
        200:
          description: OK
      tags:
      - Fleet