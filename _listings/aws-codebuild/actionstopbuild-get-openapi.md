---
swagger: "2.0"
x-collection-name: AWS CodeBuild
x-complete: 0
info:
  title: AWS CodeBuild API Stop Build
  version: 1.0.0
  description: Attempts to stop running a build.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StopBuild:
    get:
      summary: Stop Build
      description: Attempts to stop running a build.
      operationId: stopBuild
      x-api-path-slug: actionstopbuild-get
      parameters:
      - in: query
        name: id
        description: The ID of the build to attempt to stop running
        type: string
      responses:
        200:
          description: OK
      tags:
      - Builds
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