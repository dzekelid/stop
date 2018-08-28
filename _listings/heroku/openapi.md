swagger: "2.0"
x-collection-name: Heroku
x-complete: 1
info:
  title: Heroku
  description: manage-your-heroku-apps-configs-collaborators--resources
  version: "1"
host: api.heroku.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apps/{app}/ps/stop:
    parameters:
      summary: Parameters Application PS Stop
      description: Parameters application ps stop.
      operationId: parametersAppsAppPsStop
      x-api-path-slug: appsapppsstop-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Application
      - PS
      - Stop
    post:
      summary: Add Application PS Stop
      description: Stop processes of an app. Specify either ps or type to stop the
        specified processes.
      operationId: postAppsAppPsStop
      x-api-path-slug: appsapppsstop-post
      parameters:
      - in: header
        name: Accept
        description: Content type
      - in: query
        name: Accept
        description: Content type
      - in: path
        name: app
      - in: query
        name: app
        description: The app name
      - in: query
        name: ps
        description: The name of a process to stop
      - in: query
        name: type
        description: The type of process to stop
      responses:
        200:
          description: OK
      tags:
      - Application
      - PS
      - Stop