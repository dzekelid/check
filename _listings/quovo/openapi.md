---
swagger: "2.0"
x-collection-name: Quovo
x-complete: 1
info:
  title: Quovo API v3
  description: todo-add-description
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{user_id}/terms_of_use:
    get:
      summary: Check a user's TOU status
      description: "Check whether or not a User has accepted Quovo\u2019s terms of
        use."
      operationId: UsersTermsOfUseByUserIdGet
      x-api-path-slug: usersuser-idterms-of-use-get
      parameters:
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Check
      - Users
      - TOU
      - Status
---