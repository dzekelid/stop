---
swagger: "2.0"
x-collection-name: Public Transport Victoria Timetable
x-complete: 0
info:
  title: PTV Timetable API - Version 3 Get V3 Departures Route Type Route Type Stop
    Stop Route Route
  description: View departures for a specific route from a stop.
  termsOfService: http://ptv.vic.gov.au/ptv-timetable-api/
  contact:
    name: Public Transport Victoria
    url: http://ptv.vic.gov.au/digital
  version: v3
host: timetableapi.ptv.vic.gov.au
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/departures/route_type/{route_type}/stop/{stop_id}:
    get:
      summary: Get V3 Departures Route Type Route Type Stop Stop
      description: View departures for all routes from a stop.
      operationId: Departures_GetForStop
      x-api-path-slug: v3departuresroute-typeroute-typestopstop-id-get
      parameters:
      - in: query
        name: date_utc
        description: Filter by the date and time of the request (ISO 8601 UTC format)
      - in: query
        name: devid
        description: Your developer id
      - in: query
        name: direction_id
        description: Filter by identifier of direction of travel; values returned
          by Directions API - /v3/directions/route/{route_id}
      - in: query
        name: expand
        description: List objects to be returned in full (i
      - in: query
        name: gtfs
        description: Indicates that stop_id parameter will accept GTFS stop_id data
      - in: query
        name: include_cancelled
        description: Indicates if cancelled services (if they exist) are returned
          (default = false) - metropolitan train only
      - in: query
        name: max_results
        description: Maximum number of results returned
      - in: query
        name: platform_numbers
        description: Filter by platform number at stop
      - in: path
        name: route_type
        description: Number identifying transport mode; values returned via RouteTypes
          API
      - in: query
        name: signature
        description: Authentication signature for request
      - in: path
        name: stop_id
        description: Identifier of stop; values returned by Stops API
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Departures
      - Route
      - Type
      - Route
      - Type
      - Stop
      - Stop
      - Id
  /v3/departures/route_type/{route_type}/stop/{stop_id}/route/{route_id}:
    get:
      summary: Get V3 Departures Route Type Route Type Stop Stop Route Route
      description: View departures for a specific route from a stop.
      operationId: Departures_GetForStopAndRoute
      x-api-path-slug: v3departuresroute-typeroute-typestopstop-idrouteroute-id-get
      parameters:
      - in: query
        name: date_utc
        description: Filter by the date and time of the request (ISO 8601 UTC format)
      - in: query
        name: devid
        description: Your developer id
      - in: query
        name: direction_id
        description: Filter by identifier of direction of travel; values returned
          by Directions API - /v3/directions/route/{route_id}
      - in: query
        name: expand
        description: List objects to be returned in full (i
      - in: query
        name: gtfs
        description: Indicates that stop_id parameter will accept GTFS stop_id data
      - in: query
        name: include_cancelled
        description: Indicates if cancelled services (if they exist) are returned
          (default = false) - metropolitan train only
      - in: query
        name: max_results
        description: Maximum number of results returned
      - in: path
        name: route_id
        description: Identifier of route; values returned by Routes API - v3/routes
      - in: path
        name: route_type
        description: Number identifying transport mode; values returned via RouteTypes
          API
      - in: query
        name: signature
        description: Authentication signature for request
      - in: path
        name: stop_id
        description: Identifier of stop; values returned by Stops API
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Departures
      - Route
      - Type
      - Route
      - Type
      - Stop
      - Stop
      - Id
      - Route
      - Route
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