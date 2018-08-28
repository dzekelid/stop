---
swagger: "2.0"
x-collection-name: 511 Bay Area
x-complete: 0
info:
  title: Bay Area 511 Transit API Stop Timetable API
  description: San francisco 511 transit stop timetable api.
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: api.511.org
basePath: /transit
paths:
  /StopMonitoring:
    get:
      summary: Stop Monitoring API
      description: San francisco 511 transit stop monitoring api.
      operationId: StopMonitoringGet
      x-api-path-slug: stopmonitoring-get
      parameters:
      - in: query
        name: agency
      - in: query
        name: api_key
      - in: query
        name: stopCode
      responses:
        200:
          description: OK
      tags:
      - "511"
      - Stop
      - Monitoring
      - API
  /stoptimetable:
    get:
      summary: Stop Timetable API
      description: San francisco 511 transit stop timetable api.
      operationId: StoptimetableGet
      x-api-path-slug: stoptimetable-get
      parameters:
      - in: query
        name: api_key
      - in: query
        name: MonitoringRef
      - in: query
        name: OperatorRef
      responses:
        200:
          description: OK
      tags:
      - "511"
      - Stop
      - Timetable
      - API
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