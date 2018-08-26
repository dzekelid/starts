---
swagger: "2.0"
x-collection-name: CallFire
x-complete: 1
info:
  title: CallFire
  description: callfire
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /calls/broadcasts/{id}/start:
    post:
      summary: Start voice broadcast
      description: Start a voice broadcast
      operationId: startVoiceBroadcast
      x-api-path-slug: callsbroadcastsidstart-post
      parameters:
      - in: path
        name: id
        description: An id of voice broadcast to start
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
      - Start
  /texts/broadcasts/{id}/start:
    post:
      summary: Start text broadcast
      description: Starts a text broadcast
      operationId: startTextBroadcast
      x-api-path-slug: textsbroadcastsidstart-post
      parameters:
      - in: path
        name: id
        description: An id of a text broadcast to start
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Broadcasts
      - Start
---