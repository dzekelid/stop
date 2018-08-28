swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
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
  /flows/{flowName}/stop:
    post:
      summary: Post Flows Flowname Stop
      description: Post flows flowname stop.
      operationId: stopUsingPOST
      x-api-path-slug: flowsflownamestop-post
      parameters:
      - in: path
        name: flowName
        description: flowName
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowname
      - Stop