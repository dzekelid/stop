---
swagger: "2.0"
x-collection-name: Transport for London Unified
x-complete: 0
info:
  title: Transport for London Unified Stop Point  Meta  Categories
  description: Gets the list of available stoppoint additional information categories.
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
  /Line/{id}/Timetable/{fromStopPointId}/to/{toStopPointId}:
    get:
      summary: Line  Timetable from Stop Point Id to to Stop Point Id
      description: Gets the timetable for a specified station on the give line with
        specified destination.
      operationId: Line_TimetableTo
      x-api-path-slug: lineidtimetablefromstoppointidtotostoppointid-get
      parameters:
      - in: path
        name: fromStopPointId
        description: The originating stations stop point id (station naptan code e
      - in: path
        name: id
        description: A single line id e
      - in: path
        name: toStopPointId
        description: The destination stationss Naptan code
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
      - To
      - To
      - Stop
      - Point
      - Id
  /StopPoint:
    get:
      summary: Stop Point
      description: Gets a list of stoppoints within {radius} by the specified criteria.
      operationId: StopPoint_GetByGeoPoint
      x-api-path-slug: stoppoint-get
      parameters:
      - in: query
        name: categories
        description: an optional list of comma separated property categories to return
          in the StopPoints property bag
      - in: query
        name: location.lat
      - in: query
        name: location.lon
      - in: query
        name: modes
        description: the list of modes to search (comma separated mode names e
      - in: query
        name: radius
        description: 'the radius of the bounding circle in metres (default : 200)'
      - in: query
        name: returnLines
        description: true to return the lines that each stop point serves as a nested
          resource
      - in: query
        name: stopTypes
        description: a list of stopTypes that should be returned (a list of valid
          stop types can be obtained from the StopPoint/meta/stoptypes endpoint)
      - in: query
        name: useStopPointHierarchy
        description: Re-arrange the output into a parent/child hierarchy
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
  /StopPoint/Meta/Categories:
    get:
      summary: Stop Point  Meta  Categories
      description: Gets the list of available stoppoint additional information categories.
      operationId: StopPoint_MetaCategories
      x-api-path-slug: stoppointmetacategories-get
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - ""
      - Meta
      - ""
      - Categories
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