---
swagger: "2.0"
x-collection-name: AWS Directory Service
x-complete: 1
info:
  title: AWS Directory Service API
  version: 1.0.0
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
  /?Action=EnableRadius:
    get:
      summary: Enable Radius
      description: Enables multi-factor authentication (MFA) with the Remote Authentication
        Dial In User Service (RADIUS) server for an AD Connector directory.
      operationId: enableRadius
      x-api-path-slug: actionenableradius-get
      parameters:
      - in: query
        name: DirectoryId
        description: The identifier of the directory for which to enable MFA
        type: string
      - in: query
        name: RadiusSettings
        description: A RadiusSettings object that contains information about the RADIUS
          server
        type: string
      responses:
        200:
          description: OK
      tags:
      - Radius
  /?Action=UpdateRadius:
    get:
      summary: Update Radius
      description: Updates the Remote Authentication Dial In User Service (RADIUS)
        server information for an AD Connector directory.
      operationId: updateRadius
      x-api-path-slug: actionupdateradius-get
      parameters:
      - in: query
        name: DirectoryId
        description: The identifier of the directory for which to update the RADIUS
          server information
        type: string
      - in: query
        name: RadiusSettings
        description: A RadiusSettings object that contains information about the RADIUS
          server
        type: string
      responses:
        200:
          description: OK
      tags:
      - Radius
---