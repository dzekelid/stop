---
swagger: "2.0"
x-collection-name: Transport for London Unified
x-complete: 0
info:
  title: Transport for London Unified Line  Timetable from Stop Point Id
  description: Gets the timetable for a specified station on the give line.
  version: v1
host: api.tfl.gov.uk
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Line/{ids}/Arrivals/{stopPointId}:
    get:
      summary: Line s  Arrivals stop Point Id
      description: Get the list of arrival predictions for given line ids based at
        the given stop.
      operationId: Line_Arrivals
      x-api-path-slug: lineidsarrivalsstoppointid-get
      parameters:
      - in: query
        name: destinationStationId
        description: Optional
      - in: query
        name: direction
        description: Optional
      - in: path
        name: ids
        description: A comma-separated list of line ids e
      - in: path
        name: stopPointId
        description: Optional
      responses:
        200:
          description: OK
      tags:
      - Line
      - S
      - ""
      - Arrivals
      - Stop
      - Point
      - Id
  /Line/{id}/StopPoints:
    get:
      summary: Line  Stop Points
      description: Gets a list of the stations that serve the given line id.
      operationId: Line_StopPoints
      x-api-path-slug: lineidstoppoints-get
      parameters:
      - in: path
        name: id
        description: A single line id e
      - in: query
        name: tflOperatedNationalRailStationsOnly
        description: If the national-rail line is requested, this flag will filter
          the national rail stations so that only those operated by TfL are returned
      responses:
        200:
          description: OK
      tags:
      - Line
      - ""
      - Stop
      - Points
  /Line/{id}/Timetable/{fromStopPointId}:
    get:
      summary: Line  Timetable from Stop Point Id
      description: Gets the timetable for a specified station on the give line.
      operationId: Line_Timetable
      x-api-path-slug: lineidtimetablefromstoppointid-get
      parameters:
      - in: path
        name: fromStopPointId
        description: The originating stations stop point id (station naptan code e
      - in: path
        name: id
        description: A single line id e
      responses:
        200:
          description: OK
      tags:
      - Line
      - ""
      - Timetable
      - From
      - Stop
      - Point
      - Id
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