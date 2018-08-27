swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/internal/check:
    get:
      summary: Get Internal Check
      description: Get internal check.
      operationId: getV3InternalCheck
      x-api-path-slug: v3internalcheck-get
      responses:
        200:
          description: OK
      tags:
      - Internal
      - Check