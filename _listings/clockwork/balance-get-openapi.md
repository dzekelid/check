---
swagger: "2.0"
x-collection-name: Clockwork
x-complete: 0
info:
  title: Clockwork SMS Check Balance
  description: Check how much credit you have left on your account.
  termsOfService: http://www.clockworksms.com/terms-and-conditions/
  version: v1
host: api.clockworksms.com
basePath: http/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /balance:
    get:
      summary: Check Balance
      description: Check how much credit you have left on your account.
      operationId: getBalance
      x-api-path-slug: balance-get
      parameters:
      - in: query
        name: Key
        description: Your API key, available from your API account
      responses:
        200:
          description: OK
      tags:
      - Check
      - Balance
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