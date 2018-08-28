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
  /calls/broadcasts/{id}/stop:
    post:
      summary: Stop voice broadcast
      description: Stop a voice broadcast
      operationId: stopVoiceBroadcast
      x-api-path-slug: callsbroadcastsidstop-post
      parameters:
      - in: path
        name: id
        description: An id of voice broadcast to stop
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
      - Stop
  /texts/broadcasts/{id}/stop:
    post:
      summary: Stop text broadcast
      description: Stops a text broadcast
      operationId: stopTextBroadcast
      x-api-path-slug: textsbroadcastsidstop-post
      parameters:
      - in: path
        name: id
        description: An Id of a text broadcast
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Broadcasts
      - Stop