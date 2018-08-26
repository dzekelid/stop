---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 1
info:
  title: AWS EC2 Systems Manager API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StopAutomationExecution:
    get:
      summary: Stop Automation Execution
      description: Stop an Automation that is currently executing.
      operationId: stopAutomationExecution
      x-api-path-slug: actionstopautomationexecution-get
      parameters:
      - in: query
        name: AutomationExecutionId
        description: The execution ID of the Automation to stop
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Automation
      - Execution
---