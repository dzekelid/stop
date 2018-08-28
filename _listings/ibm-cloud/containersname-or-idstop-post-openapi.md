---
swagger: "2.0"
x-collection-name: IBM Cloud
x-complete: 0
info:
  title: IBM Containers Stop a single container
  description: 'Stop a single container with a given container name or ID (corresponding
    IBM Containers command: `cf ic stop <container>`).'
  version: 3.0.0
host: containers-api.ng.bluemix.net
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /containers/{name_or_id}/stop:
    post:
      summary: Stop a single container
      description: 'Stop a single container with a given container name or ID (corresponding
        IBM Containers command: `cf ic stop <container>`).'
      operationId: stop-a-single-container-with-a-given-container-name-or-id-corresponding-ibm-containers-command-cf-ic
      x-api-path-slug: containersname-or-idstop-post
      parameters:
      - in: path
        name: name_or_id
        description: The unique identifier or name of the container that you want
          to stop
      - in: query
        name: t
        description: The number of seconds to wait before the container is stopped
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Name
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