swagger: "2.0"
x-collection-name: AWS Device Farm
x-complete: 1
info:
  title: AWS Device Farm API
  version: 1.0.0
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