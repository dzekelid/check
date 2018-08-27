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
  /permission/{projectid}/{folderPath}/baseline:
    get:
      summary: Check Baseline Permission for given project
      description: Check baseline permission for given project.
      operationId: check baseline permission
      x-api-path-slug: permissionprojectidfolderpathbaseline-get
      parameters:
      - in: path
        name: folderPath
      - in: path
        name: projectPath
      responses:
        200:
          description: OK
      tags:
      - Check
      - Baseline
      - Permissiongiven
      - Project