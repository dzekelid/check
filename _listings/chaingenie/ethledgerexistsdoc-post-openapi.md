---
swagger: "2.0"
x-collection-name: ChainGenie
x-complete: 0
info:
  title: ChainGenie Check document exists on blockchain
  description: Check if your documents exists in the eth blockchain
  version: "1.0"
host: api.chaingenie.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ethledger/existsstr:
    post:
      summary: Check message exists on blockchain
      description: Check if your string exists in the eth blockchain
      operationId: EthledgerExistsstrPost
      x-api-path-slug: ethledgerexistsstr-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: str
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Check
      - Message
      - Exists
      - "On"
      - Blockchain
  /ethledger/existshash:
    post:
      summary: Check hash exists on blockchain
      description: Check if your hash exists in the eth blockchain
      operationId: EthledgerExistshashPost
      x-api-path-slug: ethledgerexistshash-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: hash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Check
      - Hash
      - Exists
      - "On"
      - Blockchain
  /ethledger/existsdoc:
    post:
      summary: Check document exists on blockchain
      description: Check if your documents exists in the eth blockchain
      operationId: EthledgerExistsdocPost
      x-api-path-slug: ethledgerexistsdoc-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: files
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Check
      - Document
      - Exists
      - "On"
      - Blockchain
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