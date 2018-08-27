---
swagger: "2.0"
x-collection-name: Pingdom
x-complete: 0
info:
  title: Results API Get Raw Check Results
  description: Return a list of raw test results for a specified check
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: api.pingdom.com
basePath: /
paths:
  ? |2-

        /api/{version}/checks
  : ? |2-

          get
    : summary: Get Check List
      description: Returns a list overview of all checks.
      operationId: |2-

        getApiVersionChecks
      x-api-path-slug: apiversionchecks-get
      parameters:
      - in: query
        name: include_tags
        description: Include tag list for each check
        type: <td>boolean</td>
      - in: query
        name: limit
        description: Limits the number of returned probes to the specified quantity
        type: <td>integer</td>
      - in: query
        name: offset
        description: Offset for listing
        type: <td>integer</td>
      - in: query
        name: tags
        description: Tag list separated by commas
        type: <td>string</td>
      responses:
        200:
          description: OK
      tags:
      - Checks
  ? |2-

        /api/{version}/results/{checkid}
  : ? |2-

          get
    : summary: Get Raw Check Results
      description: Return a list of raw test results for a specified check
      operationId: get-raw-check-results
      x-api-path-slug: apiversionresultscheckid-get
      parameters:
      - in: query
        name: from
        description: Start of period
        type: <td>integer</td>
      - in: query
        name: includeanalysis
        description: Attach available root cause analysis identifiers to corresponding
          results
        type: <td>boolean</td>
      - in: query
        name: limit
        description: Number of results to show (Will be set to 1000 if the provided
          value is greater than 1000)
        type: <td>integer</td>
      - in: query
        name: maxresponse
        description: Maximum response time (ms)
        type: <td>integer</td>
      - in: query
        name: minresponse
        description: Minimum response time (ms)
        type: <td>integer</td>
      - in: query
        name: offset
        description: Number of results to skip (Max value is 43200)
        type: <td>integer</td>
      - in: query
        name: probes
        description: Filter to only show results from a list of probes
        type: <td>string</td>
      - in: query
        name: status
        description: Filter to only show results with specified statuses
        type: <td>string</td>
      - in: query
        name: to
        description: End of period
        type: <td>integer</td>
      responses:
        200:
          description: OK
      tags:
      - Results
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