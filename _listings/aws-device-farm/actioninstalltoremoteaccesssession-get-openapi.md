---
swagger: "2.0"
x-collection-name: AWS Device Farm
x-complete: 0
info:
  title: AWS Device Farm API Install To Remote Access Session
  version: 1.0.0
  description: Installs an application to the device in a remote access session.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateRemoteAccessSession:
    get:
      summary: Create Remote Access Session
      description: Specifies and starts a remote access session.
      operationId: createRemoteAccessSession
      x-api-path-slug: actioncreateremoteaccesssession-get
      parameters:
      - in: query
        name: configuration
        description: The configuration information for the remote access session request
        type: string
      - in: query
        name: deviceArn
        description: The Amazon Resource Name (ARN) of the device for which you want
          to create a remote access session
        type: string
      - in: query
        name: name
        description: The name of the remote access session that you wish to create
        type: string
      - in: query
        name: projectArn
        description: The Amazon Resource Name (ARN) of the project for which you want
          to create a remote access session
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remote Access Sessions
  /?Action=DeleteRemoteAccessSession:
    get:
      summary: Delete Remote Access Session
      description: Deletes a completed remote access session and its results.
      operationId: deleteRemoteAccessSession
      x-api-path-slug: actiondeleteremoteaccesssession-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resource Name (ARN) of the sesssion for which you
          want to delete remote access
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remote Access Sessions
  /?Action=GetRemoteAccessSession:
    get:
      summary: Get Remote Access Session
      description: Returns a link to a currently running remote access session.
      operationId: getRemoteAccessSession
      x-api-path-slug: actiongetremoteaccesssession-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resource Name (ARN) of the remote access session about
          which you want to get session information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remote Access Sessions
  /?Action=InstallToRemoteAccessSession:
    get:
      summary: Install To Remote Access Session
      description: Installs an application to the device in a remote access session.
      operationId: installToRemoteAccessSession
      x-api-path-slug: actioninstalltoremoteaccesssession-get
      parameters:
      - in: query
        name: appArn
        description: The Amazon Resource Name (ARN) of the app about which you are
          requesting information
        type: string
      - in: query
        name: remoteAccessSessionArn
        description: The Amazon Resource Name (ARN) of the remote access session about
          which you are requesting information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remote Access Sessions
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