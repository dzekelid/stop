swagger: "2.0"
x-collection-name: CollabNet
x-complete: 1
info:
  title: Foundation API
  version: 1.0.0
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/{projectid}/roles/{roleid}/auto-grant:
    delete:
      summary: Stop granting a role automatically in a given project
      description: Stop granting a role automatically in a given project.
      operationId: removeAutoGrantRoleInProject
      x-api-path-slug: projectsprojectidrolesroleidautogrant-delete
      parameters:
      - in: path
        name: projectid
        description: Project identifier
      - in: path
        name: roleid
        description: Role identifier
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Granting
      - Role
      - Automatically
      - In
      - Given
      - Project