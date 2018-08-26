---
swagger: "2.0"
x-collection-name: Clockwork
x-complete: 1
info:
  title: Clockwork SMS
  description: the-http-interface-to-send-text-messages-can-be-accessed-using-get-or-post--all-parameters-must-be-url-encoded-and-sent-as-utf8-text-
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
---