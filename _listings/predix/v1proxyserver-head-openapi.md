---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix SAS ESP Predix Service ESP server health check
  description: API to to check health of ESP server.
  contact:
    name: zahid.iqbal2@ge.com
  version: 1.0.0
host: sas-proxy.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /monitoring/heartbeat:
    get:
      summary: Monitoring API that allows to check the ACS heartbeat
      description: Monitoring api that allows to check the acs heartbeat.
      operationId: getHeartBeatUsingGET
      x-api-path-slug: monitoringheartbeat-get
      responses:
        200:
          description: Successful response
      tags:
      - Monitoring
      - That
      - Ows
      - To
      - Check
      - ACS
      - Heartbeat
  /api/v2/execution/validation:
    post:
      summary: Validate the specified orchestration and the health of all the analytics
        used in the orchestration.
      description: To successfully validate the orchestration, the BPMN XML file must
        reference analytics that are running. The validation will call a 'healthCheck'
        entry on each analytic.  Analytics in the platform automatically have this
        entry, analytics outside the platform must implement this APIfor their validation
        to pass.  The results contain the http status for each for the healthCheck
        call to each analytic.
      operationId: validate
      x-api-path-slug: apiv2executionvalidation-post
      parameters:
      - in: body
        name: file
        description: (Required) artifact file
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Validate
      - Specified
      - Orchestration
      - Health
      - Of
      - ""
      - Analytics
      - Used
      - In
      - Orchestration
  /v1/object/checkPreregisteredObject:
    post:
      summary: Check Pre-Registered Object
      description: Check a score of Pre-Registered Object.
      operationId: check
      x-api-path-slug: v1objectcheckpreregisteredobject-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: formData
        name: individualId
        description: Individual ID
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      - in: formData
        name: registImage
        description: 'Image data(Max file size: 5MByte)'
      responses:
        200:
          description: OK
      tags:
      - Check
      - Pre-Registered
      - Object
  /v1/proxy/server:
    head:
      summary: ESP server health check
      description: API to to check health of ESP server.
      operationId: healthCheckUsingHEAD
      x-api-path-slug: v1proxyserver-head
      parameters:
      - in: body
        name: reqBody
        description: reqBody
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - ESP
      - Server
      - Health
      - Check
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