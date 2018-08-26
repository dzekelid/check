---
swagger: "2.0"
x-collection-name: AWS EC2 Container Registry Service
x-complete: 1
info:
  title: AWS EC2 Container Registry API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=BatchCheckLayerAvailability:
    get:
      summary: Batch Check Layer Availability
      description: Check the availability of multiple image layers in a specified
        registry and repository.
      operationId: batchCheckLayerAvailability
      x-api-path-slug: actionbatchchecklayeravailability-get
      parameters:
      - in: query
        name: layerDigests
        description: The digests of the image layers to check
        type: string
      - in: query
        name: registryId
        description: The AWS account ID associated with the registry that contains
          the image layers to check
        type: string
      - in: query
        name: repositoryName
        description: The name of the repository that is associated with the image
          layers to check
        type: string
      responses:
        200:
          description: OK
      tags:
      - Layer Availability
---