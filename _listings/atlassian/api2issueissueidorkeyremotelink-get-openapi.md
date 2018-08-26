---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get remote issue links
  description: Returns the remote issue links for the issue. This may be links to
    other Jira instances, web applications or web pages.
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/issue/{issueIdOrKey}/remotelink:
    get:
      summary: Get remote issue links
      description: Returns the remote issue links for the issue. This may be links
        to other Jira instances, web applications or web pages.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.getRemoteIssueLinks_get
      x-api-path-slug: api2issueissueidorkeyremotelink-get
      parameters:
      - in: query
        name: globalId
        description: ID of the remote issue link to be returned
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue to retrieve remote links for
      responses:
        200:
          description: OK
      tags:
      - Remote
      - Issue
      - Links
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