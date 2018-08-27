---
swagger: "2.0"
x-collection-name: Botify
x-complete: 0
info:
  title: Botify Get Analyses Username Project Slug Analysis Slug Urls Export Url Export
  description: Checks the status of an CSVUrlExportJob object. Returns json object
    with the status.
  version: 1.0.0
host: api.botify.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /analyses/{username}/{project_slug}/{analysis_slug}/urls/export/{url_export_id}:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Urls Export Url Export
      description: Checks the status of an CSVUrlExportJob object. Returns json object
        with the status.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugUrlsExportUrlExport
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlsexporturl-export-id-get
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Export
      - Url
      - Export
      - Id
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