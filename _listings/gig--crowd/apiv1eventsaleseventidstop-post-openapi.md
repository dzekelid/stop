---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Post Event Sales Eventid Stop
  version: 1.0.0
  description: Post event sales eventid stop.
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