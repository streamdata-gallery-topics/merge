---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Merge versions
  description: Merges two project versions. The merge is completed by deleting the
    version specified in `id` and replacing any occurrences of its ID in `fixVersion`
    with the version ID specified in `moveIssuesTo`. Consider using [Delete and replace
    version](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-version-id-removeAndSwap-post)
    instead. This resource supports swapping version values in `fixVersion`, `affectedVersion`,
    and custom fields. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg)
    or _Administer Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
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
  /api/2/version/{id}/mergeto/{moveIssuesTo}:
    put:
      summary: Merge versions
      description: Merges two project versions. The merge is completed by deleting
        the version specified in `id` and replacing any occurrences of its ID in `fixVersion`
        with the version ID specified in `moveIssuesTo`. Consider using [Delete and
        replace version](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-version-id-removeAndSwap-post)
        instead. This resource supports swapping version values in `fixVersion`, `affectedVersion`,
        and custom fields. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg)
        or _Administer Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
      operationId: com.atlassian.jira.rest.v2.issue.VersionResource.mergeVersions_put
      x-api-path-slug: api2versionidmergetomoveissuesto-put
      parameters:
      - in: path
        name: id
        description: The ID of the version to delete
      - in: path
        name: moveIssuesTo
        description: The ID of the version to merge into
      responses:
        200:
          description: OK
      tags:
      - Merge
      - Versions
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