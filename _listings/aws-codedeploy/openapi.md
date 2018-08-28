swagger: "2.0"
x-collection-name: AWS CodeDeploy
x-complete: 1
info:
  title: AWS CodeDeploy API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StopDeployment:
    get:
      summary: Stop Deployment
      description: Attempts to stop an ongoing deployment.
      operationId: stopDeployment
      x-api-path-slug: actionstopdeployment-get
      parameters:
      - in: query
        name: autoRollbackEnabled
        description: Indicates, when a deployment is stopped, whether instances that
          have been updated            should be rolled back to the previous version
          of the application revision
        type: string
      - in: query
        name: deploymentId
        description: The unique ID of a deployment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployments