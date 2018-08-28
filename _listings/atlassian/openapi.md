swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
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
    post:
      summary: Create or update remote issue link
      description: Creates or updates a remote issue link from a JSON representation.
        If a `globalId` is provided and a remote issue link exists with that globalId,
        the remote issue link is updated. Otherwise, the remote issue link is created.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.createOrUpdateRemoteIssueLink_post
      x-api-path-slug: api2issueissueidorkeyremotelink-post
      parameters:
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue to create/update the remote issue link
          for
      responses:
        200:
          description: OK
      tags:
      - Update
      - Remote
      - Issue
      - Link
    delete:
      summary: Delete remote issue link by global id
      description: Deletes the issue's remote link with the given global ID.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.deleteRemoteIssueLinkByGlobalId_delete
      x-api-path-slug: api2issueissueidorkeyremotelink-delete
      parameters:
      - in: query
        name: globalId
        description: Global ID of a remote issue link to delete
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue to delete a remote issue link for
      responses:
        200:
          description: OK
      tags:
      - Remote
      - Issue
      - Link
      - By
      - Global
      - Id
  /api/2/issue/{issueIdOrKey}/remotelink/{linkId}:
    get:
      summary: Get remote issue link by id
      description: Returns the remote issue link by the given ID.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.getRemoteIssueLinkById_get
      x-api-path-slug: api2issueissueidorkeyremotelinklinkid-get
      parameters:
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue to retrieve the remote issue links for
      - in: path
        name: linkId
        description: ID of the remote issue link
      responses:
        200:
          description: OK
      tags:
      - Remote
      - Issue
      - Link
      - By
      - Id
    put:
      summary: Update remote issue link
      description: Updates a remote issue link from a JSON representation. Sets all
        fields without values provided to null.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.updateRemoteIssueLink_put
      x-api-path-slug: api2issueissueidorkeyremotelinklinkid-put
      parameters:
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue to update the remote issue link for
      - in: path
        name: linkId
      responses:
        200:
          description: OK
      tags:
      - Remote
      - Issue
      - Link
    delete:
      summary: Delete remote issue link by id
      description: Deletes the issue's remote link with the given ID.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.deleteRemoteIssueLinkById_delete
      x-api-path-slug: api2issueissueidorkeyremotelinklinkid-delete
      parameters:
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue to delete a remote issue link for
      - in: path
        name: linkId
        description: ID of a remote issue link to delete
      responses:
        200:
          description: OK
      tags:
      - Remote
      - Issue
      - Link
      - By
      - Id
  /api/2/version/remotelink:
    get:
      summary: Get remote version links
      description: Returns the remote version links for a given global ID.
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.getRemoteVersionLinks_get
      x-api-path-slug: api2versionremotelink-get
      parameters:
      - in: query
        name: globalId
        description: the global ID of the remote resource that is linked to the versions
      responses:
        200:
          description: OK
      tags:
      - Remote
      - Version
      - Links
  /api/2/version/{versionId}/remotelink:
    get:
      summary: Get remote version links by version id
      description: Returns the remote version links associated with the given version
        ID.
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.getRemoteVersionLinksByVersionId_get
      x-api-path-slug: api2versionversionidremotelink-get
      parameters:
      - in: path
        name: versionId
        description: a String containing the version ID
      responses:
        200:
          description: OK
      tags:
      - Remote
      - Version
      - Links
      - By
      - Version
      - Id
    post:
      summary: Create or update remote version link
      description: Create a remote version link via POST. The link's global ID will
        be taken from the JSON payload if provided; otherwise, it will be generated.
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.createOrUpdateRemoteVersionLink_post
      x-api-path-slug: api2versionversionidremotelink-post
      parameters:
      - in: path
        name: versionId
      responses:
        200:
          description: OK
      tags:
      - Update
      - Remote
      - Version
      - Link
    delete:
      summary: Delete remote version links by version id
      description: Delete all remote version links for a given version ID.
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.deleteRemoteVersionLinksByVersionId_delete
      x-api-path-slug: api2versionversionidremotelink-delete
      parameters:
      - in: path
        name: versionId
        description: The version for which to delete ALL existing remote version links
      responses:
        200:
          description: OK
      tags:
      - Remote
      - Version
      - Links
      - By
      - Version
      - Id
  /api/2/version/{versionId}/remotelink/{globalId}:
    get:
      summary: Get remote version link
      description: A REST sub-resource representing a remote version link
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.getRemoteVersionLink_get
      x-api-path-slug: api2versionversionidremotelinkglobalid-get
      parameters:
      - in: path
        name: globalId
        description: The id of the remote issue link to be returned
      - in: path
        name: versionId
        description: a String containing the version id
      responses:
        200:
          description: OK
      tags:
      - Remote
      - Version
      - Link
    post:
      summary: Create or update remote version link with global id
      description: Create a remote version link via POST using the provided global
        ID.
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.createOrUpdateRemoteVersionLinkWithGlobalId_post
      x-api-path-slug: api2versionversionidremotelinkglobalid-post
      parameters:
      - in: path
        name: globalId
      - in: path
        name: versionId
      responses:
        200:
          description: OK
      tags:
      - Update
      - Remote
      - Version
      - Link
      - Global
      - Id
    delete:
      summary: Delete remote version link
      description: Delete a specific remote version link with the given version ID
        and global ID.
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.deleteRemoteVersionLink_delete
      x-api-path-slug: api2versionversionidremotelinkglobalid-delete
      parameters:
      - in: path
        name: globalId
        description: The global ID of the remote link
      - in: path
        name: versionId
        description: The version ID of the remote link
      responses:
        200:
          description: OK
      tags:
      - Remote
      - Version
      - Link