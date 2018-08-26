---
swagger: "2.0"
x-collection-name: AWS Device Farm
x-complete: 0
info:
  title: AWS Device Farm API Stop Run
  version: 1.0.0
  description: Initiates a stop request for the current test run.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StopRemoteAccessSession:
    get:
      summary: Stop Remote Access Session
      description: Ends a specified remote access session.
      operationId: stopRemoteAccessSession
      x-api-path-slug: actionstopremoteaccesssession-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resource Name (ARN) of the remote access session you
          wish to stop
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remote Access Sessions
  /?Action=StopRun:
    get:
      summary: Stop Run
      description: Initiates a stop request for the current test run.
      operationId: stopRun
      x-api-path-slug: actionstoprun-get
      parameters:
      - in: query
        name: arn
        description: Represents the Amazon Resource Name (ARN) of the Device Farm
          run you wish to stop
        type: string
      responses:
        200:
          description: OK
      tags:
      - Runs
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