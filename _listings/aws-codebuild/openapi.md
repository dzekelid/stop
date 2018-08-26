---
swagger: "2.0"
x-collection-name: AWS CodeBuild
x-complete: 1
info:
  title: AWS CodeBuild API
  version: 1.0.0
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
---