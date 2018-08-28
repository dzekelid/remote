---
swagger: "2.0"
x-collection-name: AWS Directory Service
x-complete: 0
info:
  title: AWS Directory Service API Disable Radius
  version: 1.0.0
  description: Disables multi-factor authentication (MFA) with the Remote Authentication
    Dial In User Service (RADIUS) server for an AD Connector directory.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DisableRadius:
    get:
      summary: Disable Radius
      description: Disables multi-factor authentication (MFA) with the Remote Authentication
        Dial In User Service (RADIUS) server for an AD Connector directory.
      operationId: disableRadius
      x-api-path-slug: actiondisableradius-get
      parameters:
      - in: query
        name: DirectoryId
        description: The identifier of the directory for which to disable MFA
        type: string
      responses:
        200:
          description: OK
      tags:
      - Radius
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