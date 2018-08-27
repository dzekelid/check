swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost
  version: 1.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/mfa:
    post:
      summary: Check MFA
      description: |-
        Check if a user has multi-factor authentication active on their account by providing a login id. Used to check whether an MFA code needs to be provided when logging in.
        ##### Permissions
        No permission required.
      operationId: check-if-a-user-has-multifactor-authentication-active-on-their-account-by-providing-a-login-id-used-
      x-api-path-slug: usersmfa-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Check
      - MFA
  /teams/name/{name}/exists:
    get:
      summary: Check if team exists
      description: Check if the team exists based on a team name.
      operationId: check-if-the-team-exists-based-on-a-team-name
      x-api-path-slug: teamsnamenameexists-get
      parameters:
      - in: path
        name: name
        description: Team Name
      responses:
        200:
          description: OK
      tags:
      - Check
      - If
      - Team
      - Exists
  /system/ping:
    get:
      summary: Check system health
      description: |-
        Check if the server is up and healthy based on the configuration setting `GoRoutineHealthThreshold`. If `GoRoutineHealthThreshold` and the number of goroutines on the server exceeds that threshold the server is considered unhealthy. If `GoRoutineHealthThreshold` is not set or the number of goroutines is below the threshold the server is considered healthy.
        __Minimum server version__: 3.10
        ##### Permissions
        Must be logged in.
      operationId: check-if-the-server-is-up-and-healthy-based-on-the-configuration-setting-goroutinehealththreshold-if
      x-api-path-slug: systemping-get
      responses:
        200:
          description: OK
      tags:
      - Check
      - System
      - Health