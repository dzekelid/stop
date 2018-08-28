---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Insights Post Flow Templates Flowtemplateid Flows Flowid Stop
  description: Post flow templates flowtemplateid flows flowid stop.
  termsOfService: urn:tos
  version: 1.0.0
host: insights-api.data-services.predix.io
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /flow-templates/{flowTemplateId}/flows/{flowId}/stop:
    post:
      summary: Post Flow Templates Flowtemplateid Flows Flowid Stop
      description: Post flow templates flowtemplateid flows flowid stop.
      operationId: stopUsingPOST_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowidstop-post
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
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