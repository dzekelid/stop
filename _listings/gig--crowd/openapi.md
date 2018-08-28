swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/event/sales/{eventId}/stop:
    post:
      summary: Post Event Sales Eventid Stop
      description: Post event sales eventid stop.
      operationId: postApiV1EventSalesEventStop
      x-api-path-slug: apiv1eventsaleseventidstop-post
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: eventId
      responses:
        200:
          description: OK
      tags:
      - Event
      - Sales
      - Eventid
      - Stop