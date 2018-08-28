swagger: "2.0"
x-collection-name: MockLab
x-complete: 1
info:
  title: WireMock
  version: 1.0.0
basePath: /__admin
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /recordings/stop:
    post:
      summary: Post Recordings Stop
      description: Stop recording stub mappings
      operationId: postRecordingsStop
      x-api-path-slug: recordingsstop-post
      responses:
        200:
          description: Successful response
      tags:
      - Recordings
      - Stop