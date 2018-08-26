---
swagger: "2.0"
x-collection-name: MotaWord
x-complete: 1
info:
  title: Mota Word
  description: use-motaword-api-to-post-and-track-your-translation-projects-
  version: alpha-0.1.0
host: api.motaword.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/{id}/package/check:
    get:
      summary: Track the status of translation packaging.
      description: This request will tell you the current progress of the translation
        packaging. You will use the 'key' provided by the /package call.
      operationId: trackPackage
      x-api-path-slug: projectsidpackagecheck-get
      parameters:
      - in: path
        name: id
        description: Project ID
      - in: query
        name: key
        description: This is the package tracking key provided in the response of
          a /package call
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Package
      - Check
---