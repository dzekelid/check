---
swagger: "2.0"
x-collection-name: Slack
x-complete: 1
info:
  title: Slack
  description: one-way-to-interact-with-the-slack-platform-is-its-http-rpcbased-web-api-a-collection-of-methods-requiring-oauth-2-0based-user-bot-or-workspace-tokens-blessed-with-related-oauth-scopes-
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
---