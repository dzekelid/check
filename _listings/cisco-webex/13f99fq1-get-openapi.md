---
swagger: "2.0"
x-collection-name: Cisco WebEx
x-complete: 0
info:
  title: WebEx Teams API Check requestb.in (test purpose)
  description: check an event has been posted
  version: 1.0.0
host: api.ciscospark.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /13f99fq1:
    get:
      summary: Check requestb.in (test purpose)
      description: check an event has been posted
      operationId: 13f99fq1Get
      x-api-path-slug: 13f99fq1-get
      parameters:
      - in: query
        name: inspect
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Check
      - Requestb
      - In
      - (test
      - Purpose)
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