---
swagger: "2.0"
x-collection-name: Urban Airship
x-complete: 1
info:
  title: Urban Airship
  description: the-urban-airships-api-powers-mobile-applications-with-push-rich-push-inapp-purchases-and-subscription-services-
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
---