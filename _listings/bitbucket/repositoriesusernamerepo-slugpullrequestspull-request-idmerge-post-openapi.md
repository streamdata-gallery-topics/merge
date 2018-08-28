---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Add Repositories Username Repo Slug Pullrequests Pull Request  Merge
  description: Post repositories username repo slug pullrequests pull request  merge
  termsOfService: https://www.atlassian.com/legal/customer-agreement
  contact:
    name: Bitbucket Support
    url: https://support.atlassian.com/bitbucket
    email: support@bitbucket.org
  version: 1.0.0
host: api.bitbucket.org
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repositories/{username}/{repo_slug}/pullrequests/{pull_request_id}/merge:
    parameters:
      summary: Parameters Repositories Username Repo Slug Pullrequests Pull Request  Merge
      description: Parameters repositories username repo slug pullrequests pull request  merge
      operationId: parametersRepositoriesUsernameRepoSlugPullrequestsPullRequestMerge
      x-api-path-slug: repositoriesusernamerepo-slugpullrequestspull-request-idmerge-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pullrequests
      - Pull
      - Request
      - ""
      - Merge
    post:
      summary: Add Repositories Username Repo Slug Pullrequests Pull Request  Merge
      description: Post repositories username repo slug pullrequests pull request  merge
      operationId: postRepositoriesUsernameRepoSlugPullrequestsPullRequestMerge
      x-api-path-slug: repositoriesusernamerepo-slugpullrequestspull-request-idmerge-post
      parameters:
      - in: body
        name: _body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pullrequests
      - Pull
      - Request
      - ""
      - Merge
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