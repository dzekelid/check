---
swagger: "2.0"
x-collection-name: Urban Airship
x-complete: 0
info:
  title: Urban Airship Post App Updates
  description: Checks for updates. It can be useful on application launch to compare
    a list of installed updates with our server to see if there are any updates to
    be had for the content.
  version: v3
host: go.urbanairship.com
basePath: /api/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /app/updates:
    post:
      summary: Post App Updates
      description: Checks for updates. It can be useful on application launch to compare
        a list of installed updates with our server to see if there are any updates
        to be had for the content.
      operationId: app.updates.post
      x-api-path-slug: appupdates-post
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: product_id
        description: The product ID
      responses:
        200:
          description: OK
      tags:
      - App
      - Updates
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