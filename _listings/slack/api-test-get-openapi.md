---
swagger: "2.0"
x-collection-name: Slack
x-complete: 0
info:
  title: Slack Test API
  description: Checks API calling code.
  version: 1.0.3
host: slack.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api.test:
    get:
      summary: Test API
      description: Checks API calling code.
      operationId: api_test
      x-api-path-slug: api-test-get
      parameters:
      - in: query
        name: error
        description: Error response to return
      - in: query
        name: foo
        description: example property to return
      responses:
        200:
          description: OK
      tags:
      - Messaging
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