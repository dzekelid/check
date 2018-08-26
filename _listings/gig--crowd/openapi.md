---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/phone/check/{smsId}:
    get:
      summary: Get Phone Check Smsid
      description: Get phone check smsid.
      operationId: getApiV1PhoneCheckSms
      x-api-path-slug: apiv1phonechecksmsid-get
      parameters:
      - in: path
        name: smsId
      responses:
        200:
          description: OK
      tags:
      - Phone
      - Check
      - Smsid
---