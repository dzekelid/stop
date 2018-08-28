swagger: "2.0"
x-collection-name: AWS WorkSpaces
x-complete: 1
info:
  title: AWS WorkSpaces Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ModifyWorkspaceProperties:
    get:
      summary: Modify Workspace Properties
      description: Modifies the WorkSpace properties, including the running mode and
        AutoStop time.
      operationId: modifyWorkspaceProperties
      x-api-path-slug: actionmodifyworkspaceproperties-get
      parameters:
      - in: query
        name: WorkspaceId
        description: The ID of the WorkSpace
        type: string
      - in: query
        name: WorkspaceProperties
        description: The WorkSpace properties of the request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Workspaces
  /?Action=StopWorkspaces:
    get:
      summary: Stop Workspaces
      description: Stops the specified WorkSpaces.
      operationId: stopWorkspaces
      x-api-path-slug: actionstopworkspaces-get
      parameters:
      - in: query
        name: StopWorkspaceRequests
        description: The requests
        type: string
      responses:
        200:
          description: OK
      tags:
      - Workspaces