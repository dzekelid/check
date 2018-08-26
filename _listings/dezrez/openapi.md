---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/branch/checkkeycodesexist:
    get:
      summary: Check specified key codes exist in branch
      description: Check specified key codes exist in branch.
      operationId: Branch_CheckKeycodesExistBykeyCodes
      x-api-path-slug: apibranchcheckkeycodesexist-get
      parameters:
      - in: query
        name: keyCodes
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Check
      - Specified
      - Key
      - Codes
      - Exist
      - In
      - Branch
  /api/credentials/emailsync/usernamepassword:
    post:
      summary: "Creates or Updates Email Sync Security Credentials\r\nThis also uses
        the credentials to do a quick check and see if they are working\r\nit will
        throw an internal server error if there is an issue with the connection\r\nbut
        this may be the server address (s"
      description: "Creates or updates email sync security credentials\r\nthis also
        uses the credentials to do a quick check and see if they are working\r\nit
        will throw an internal server error if there is an issue with the connection\r\nbut
        this may be the server address (s."
      operationId: Credentials_UpsertEmailSyncUsernamePasswordBycredentialDataContract
      x-api-path-slug: apicredentialsemailsyncusernamepassword-post
      parameters:
      - in: body
        name: credentialDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - S
      - Email
      - Sync
      - Security
      - "Credentials\r\nThis"
      - Also
      - Uses
      - Credentials
      - To
      - Do
      - Quick
      - Check
      - See
      - If
      - They
      - Are
      - "Working\r\nIt"
      - Will
      - Throw
      - Internal
      - Server
      - Error
      - If
      - There
      - Is
      - Issue
      - "Connection\r\nBut"
      - This
      - May
      - Be
      - Server
      - Address
      - (s
  /api/sync/calendarsyncenabled:
    get:
      summary: "check if the calendar sync is enabled for this user\r\nthis could
        be used to enabled/disable the calendar setup button"
      description: "Check if the calendar sync is enabled for this user\r\nthis could
        be used to enabled/disable the calendar setup button."
      operationId: Sync_CalendarSyncEnabled
      x-api-path-slug: apisynccalendarsyncenabled-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Check
      - If
      - Calendar
      - Sync
      - Is
      - Enabledthis
      - "User\r\nThis"
      - Could
      - Be
      - Used
      - To
      - Enabled
      - Disable
      - Calendar
      - Setup
      - Button
  /api/sync/mailsyncanddraftenabled:
    get:
      summary: "check if they user has setup their credentials for smap services\r\nthis
        could be used to enabled/disable the mail sync button"
      description: "Check if they user has setup their credentials for smap services\r\nthis
        could be used to enabled/disable the mail sync button."
      operationId: Sync_MailSyncAndDraftEnabled
      x-api-path-slug: apisyncmailsyncanddraftenabled-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Check
      - If
      - They
      - User
      - Has
      - Setup
      - Their
      - Credentialssmap
      - "Services\r\nThis"
      - Could
      - Be
      - Used
      - To
      - Enabled
      - Disable
      - Mail
      - Sync
      - Button
  /api/sync/mailsendenabled:
    get:
      summary: check if the user has setup their credientials for smtp services
      description: Check if the user has setup their credientials for smtp services.
      operationId: Sync_MailSendEnabled
      x-api-path-slug: apisyncmailsendenabled-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Check
      - If
      - User
      - Has
      - Setup
      - Their
      - Credientialssmtp
      - Services
  /api/sync/imapserversetup:
    get:
      summary: check if the user has setup their credientials for smtp services
      description: Check if the user has setup their credientials for smtp services.
      operationId: Sync_ImapServerSetup
      x-api-path-slug: apisyncimapserversetup-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Check
      - If
      - User
      - Has
      - Setup
      - Their
      - Credientialssmtp
      - Services
  /api/inboundlead/checkformatchinggroups:
    get:
      summary: Check for Matching groups for the given leads based on contact item
        values i.e. Emails and Phones.
      description: Check for matching groups for the given leads based on contact
        item values i.e. emails and phones..
      operationId: InboundLead_CheckForMatchingGroupsByleadIdBypageSizeBypageNumber
      x-api-path-slug: apiinboundleadcheckformatchinggroups-get
      parameters:
      - in: query
        name: leadId
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - CheckMatching
      - Groupsthe
      - Given
      - Leads
      - Based
      - "On"
      - Contact
      - Item
      - Values
      - I
      - E
      - ""
      - Emails
      - Phones
  /api/property/{id}/keys/checkin:
    put:
      summary: Checkin a collection of keys for a property
      description: Checkin a collection of keys for a property.
      operationId: Property_CheckinKeysByidBycheckinDetails
      x-api-path-slug: apipropertyidkeyscheckin-put
      parameters:
      - in: body
        name: checkinDetails
        description: The details of the keys to checkin
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Checkin
      - Collection
      - Of
      - Keysa
      - Property
  /api/property/{id}/keys/checkout:
    put:
      summary: Checkout a collection of keys for a property
      description: Checkout a collection of keys for a property.
      operationId: Property_CheckoutKeysByidBycheckoutDetails
      x-api-path-slug: apipropertyidkeyscheckout-put
      parameters:
      - in: body
        name: checkoutDetails
        description: The details of the keys to checkout
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Checkout
      - Collection
      - Of
      - Keysa
      - Property
---