---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Get Projects Merge Request Merge Request Comments
  version: 1.0.0
  description: Get projects merge request merge request comments.
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/merge_requests/{merge_request_id}/award_emoji:
    get:
      summary: Get Projects Merge Requests Merge Request Award Emoji
      description: Get projects merge requests merge request award emoji.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestIdAwardEmoji
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idaward-emoji-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
        description: The ID of an Issue, Merge Request or Snippet
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Award
      - Emoji
    post:
      summary: Post Projects Merge Requests Merge Request Award Emoji
      description: Post projects merge requests merge request award emoji.
      operationId: postV3ProjectsIdMergeRequestsMergeRequestIdAwardEmoji
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idaward-emoji-post
      parameters:
      - in: path
        name: id
      - in: path
        name: merge_request_id
      - in: formData
        name: name
        description: The name of a award_emoji (without colons)
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Award
      - Emoji
  /v3/projects/{id}/merge_requests/{merge_request_id}/award_emoji/{award_id}:
    get:
      summary: Get Projects Merge Requests Merge Request Award Emoji Award
      description: Get projects merge requests merge request award emoji award.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestIdAwardEmojiAwardId
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idaward-emojiaward-id-get
      parameters:
      - in: path
        name: award_id
        description: The ID of the award
      - in: path
        name: id
      - in: path
        name: merge_request_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Award
      - Emoji
      - Award
    delete:
      summary: Delete Projects Merge Requests Merge Request Award Emoji Award
      description: Delete projects merge requests merge request award emoji award.
      operationId: deleteV3ProjectsIdMergeRequestsMergeRequestIdAwardEmojiAwardId
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idaward-emojiaward-id-delete
      parameters:
      - in: path
        name: award_id
        description: The ID of an award emoji
      - in: path
        name: id
      - in: path
        name: merge_request_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Award
      - Emoji
      - Award
  /v3/projects/{id}/merge_requests/{merge_request_id}/notes/{note_id}/award_emoji:
    get:
      summary: Get Projects Merge Requests Merge Request Notes Note Award Emoji
      description: Get projects merge requests merge request notes note award emoji.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestIdNotesNoteIdAwardEmoji
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idnotesnote-idaward-emoji-get
      parameters:
      - in: path
        name: id
      - in: path
        name: merge_request_id
      - in: path
        name: note_id
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Notes
      - Note
      - Award
      - Emoji
    post:
      summary: Post Projects Merge Requests Merge Request Notes Note Award Emoji
      description: Post projects merge requests merge request notes note award emoji.
      operationId: postV3ProjectsIdMergeRequestsMergeRequestIdNotesNoteIdAwardEmoji
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idnotesnote-idaward-emoji-post
      parameters:
      - in: path
        name: id
      - in: path
        name: merge_request_id
      - in: formData
        name: name
        description: The name of a award_emoji (without colons)
      - in: path
        name: note_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Notes
      - Note
      - Award
      - Emoji
  /v3/projects/{id}/merge_requests/{merge_request_id}/notes/{note_id}/award_emoji/{award_id}:
    get:
      summary: Get Projects Merge Requests Merge Request Notes Note Award Emoji Award
      description: Get projects merge requests merge request notes note award emoji
        award.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestIdNotesNoteIdAwardEmojiAwardId
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idnotesnote-idaward-emojiaward-id-get
      parameters:
      - in: path
        name: award_id
        description: The ID of the award
      - in: path
        name: id
      - in: path
        name: merge_request_id
      - in: path
        name: note_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Notes
      - Note
      - Award
      - Emoji
      - Award
    delete:
      summary: Delete Projects Merge Requests Merge Request Notes Note Award Emoji
        Award
      description: Delete projects merge requests merge request notes note award emoji
        award.
      operationId: deleteV3ProjectsIdMergeRequestsMergeRequestIdNotesNoteIdAwardEmojiAwardId
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idnotesnote-idaward-emojiaward-id-delete
      parameters:
      - in: path
        name: award_id
        description: The ID of an award emoji
      - in: path
        name: id
      - in: path
        name: merge_request_id
      - in: path
        name: note_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Notes
      - Note
      - Award
      - Emoji
      - Award
  /v3/projects/{id}/merge_requests/{merge_request_id}/versions:
    get:
      summary: Get Projects Merge Requests Merge Request Versions
      description: Get projects merge requests merge request versions.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestIdVersions
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idversions-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
        description: The ID of a merge request
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Versions
  /v3/projects/{id}/merge_requests/{merge_request_id}/versions/{version_id}:
    get:
      summary: Get Projects Merge Requests Merge Request Versions Version
      description: Get projects merge requests merge request versions version.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestIdVersionsVersionId
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idversionsversion-id-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
        description: The ID of a merge request
      - in: path
        name: version_id
        description: The ID of a merge request diff version
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Versions
      - Version
  /v3/projects/{id}/merge_requests/{merge_request_id}/time_estimate:
    post:
      summary: Post Projects Merge Requests Merge Request Time Estimate
      description: Post projects merge requests merge request time estimate.
      operationId: postV3ProjectsIdMergeRequestsMergeRequestIdTimeEstimate
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idtime-estimate-post
      parameters:
      - in: formData
        name: duration
        description: The duration to be parsed
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
        description: The ID of a project merge_request
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Time
      - Estimate
  /v3/projects/{id}/merge_requests/{merge_request_id}/reset_time_estimate:
    post:
      summary: Post Projects Merge Requests Merge Request Reset Time Estimate
      description: Post projects merge requests merge request reset time estimate.
      operationId: postV3ProjectsIdMergeRequestsMergeRequestIdResetTimeEstimate
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idreset-time-estimate-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
        description: The ID of a project merge_request
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Reset
      - Time
      - Estimate
  /v3/projects/{id}/merge_requests/{merge_request_id}/add_spent_time:
    post:
      summary: Post Projects Merge Requests Merge Request Add Spent Time
      description: Post projects merge requests merge request add spent time.
      operationId: postV3ProjectsIdMergeRequestsMergeRequestIdAddSpentTime
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idadd-spent-time-post
      parameters:
      - in: formData
        name: duration
        description: The duration to be parsed
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
        description: The ID of a project merge_request
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - ""
      - Spent
      - Time
  /v3/projects/{id}/merge_requests/{merge_request_id}/reset_spent_time:
    post:
      summary: Post Projects Merge Requests Merge Request Reset Spent Time
      description: Post projects merge requests merge request reset spent time.
      operationId: postV3ProjectsIdMergeRequestsMergeRequestIdResetSpentTime
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idreset-spent-time-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
        description: The ID of a project merge_request
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Reset
      - Spent
      - Time
  /v3/projects/{id}/merge_requests/{merge_request_id}/time_stats:
    get:
      summary: Get Projects Merge Requests Merge Request Time Stats
      description: Get projects merge requests merge request time stats.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestIdTimeStats
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idtime-stats-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
        description: The ID of a project merge_request
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Time
      - Stats
  /v3/projects/{id}/merge_requests:
    get:
      summary: Get Projects Merge Requests
      description: Get projects merge requests.
      operationId: getV3ProjectsIdMergeRequests
      x-api-path-slug: v3projectsidmerge-requests-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: iid
        description: The IID of the merge requests
      - in: query
        name: order_by
        description: Return merge requests ordered by `created_at` or `updated_at`
          fields
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: sort
        description: Return merge requests sorted in `asc` or `desc` order
      - in: query
        name: state
        description: Return opened, closed, merged, or all merge requests
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
    post:
      summary: Post Projects Merge Requests
      description: Post projects merge requests.
      operationId: postV3ProjectsIdMergeRequests
      x-api-path-slug: v3projectsidmerge-requests-post
      parameters:
      - in: formData
        name: assignee_id
        description: The ID of a user to assign the merge request
      - in: formData
        name: description
        description: The description of the merge request
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: labels
        description: Comma-separated list of label names
      - in: formData
        name: milestone_id
        description: The ID of a milestone to assign the merge request
      - in: formData
        name: remove_source_branch
        description: Remove source branch when merging
      - in: formData
        name: source_branch
        description: The source branch
      - in: formData
        name: target_branch
        description: The target branch
      - in: formData
        name: target_project_id
        description: The target project of the merge request defaults to the :id of
          the project
      - in: formData
        name: title
        description: The title of the merge request
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
  /v3/projects/{id}/merge_requests/{merge_request_id}:
    delete:
      summary: Delete Projects Merge Requests Merge Request
      description: Delete projects merge requests merge request.
      operationId: deleteV3ProjectsIdMergeRequestsMergeRequestId
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-id-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
        description: The ID of a merge request
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
    get:
      summary: Get Projects Merge Requests Merge Request
      description: Get projects merge requests merge request.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestId
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-id-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
    put:
      summary: Put Projects Merge Requests Merge Request
      description: Put projects merge requests merge request.
      operationId: putV3ProjectsIdMergeRequestsMergeRequestId
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-id-put
      parameters:
      - in: formData
        name: assignee_id
        description: The ID of a user to assign the merge request
      - in: formData
        name: description
        description: The description of the merge request
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: labels
        description: Comma-separated list of label names
      - in: path
        name: merge_request_id
      - in: formData
        name: milestone_id
        description: The ID of a milestone to assign the merge request
      - in: formData
        name: remove_source_branch
        description: Remove source branch when merging
      - in: formData
        name: state_event
        description: Status of the merge request
      - in: formData
        name: target_branch
        description: The target branch
      - in: formData
        name: title
        description: The title of the merge request
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
  /v3/projects/{id}/merge_request/{merge_request_id}:
    get:
      summary: Get Projects Merge Request Merge Request
      description: This endpoint is deprecated and will be removed in GitLab 9.0.
      operationId: getV3ProjectsIdMergeRequestMergeRequestId
      x-api-path-slug: v3projectsidmerge-requestmerge-request-id-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
        description: The ID of a merge request
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Merge
      - Request
    put:
      summary: Put Projects Merge Request Merge Request
      description: Put projects merge request merge request.
      operationId: putV3ProjectsIdMergeRequestMergeRequestId
      x-api-path-slug: v3projectsidmerge-requestmerge-request-id-put
      parameters:
      - in: formData
        name: assignee_id
        description: The ID of a user to assign the merge request
      - in: formData
        name: description
        description: The description of the merge request
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: labels
        description: Comma-separated list of label names
      - in: path
        name: merge_request_id
      - in: formData
        name: milestone_id
        description: The ID of a milestone to assign the merge request
      - in: formData
        name: remove_source_branch
        description: Remove source branch when merging
      - in: formData
        name: state_event
        description: Status of the merge request
      - in: formData
        name: target_branch
        description: The target branch
      - in: formData
        name: title
        description: The title of the merge request
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Merge
      - Request
  /v3/projects/{id}/merge_request/{merge_request_id}/commits:
    get:
      summary: Get Projects Merge Request Merge Request Commits
      description: Get projects merge request merge request commits.
      operationId: getV3ProjectsIdMergeRequestMergeRequestIdCommits
      x-api-path-slug: v3projectsidmerge-requestmerge-request-idcommits-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Merge
      - Request
      - Commits
  /v3/projects/{id}/merge_request/{merge_request_id}/changes:
    get:
      summary: Get Projects Merge Request Merge Request Changes
      description: Get projects merge request merge request changes.
      operationId: getV3ProjectsIdMergeRequestMergeRequestIdChanges
      x-api-path-slug: v3projectsidmerge-requestmerge-request-idchanges-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Merge
      - Request
      - Changes
  /v3/projects/{id}/merge_request/{merge_request_id}/merge:
    put:
      summary: Put Projects Merge Request Merge Request Merge
      description: Put projects merge request merge request merge.
      operationId: putV3ProjectsIdMergeRequestMergeRequestIdMerge
      x-api-path-slug: v3projectsidmerge-requestmerge-request-idmerge-put
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: merge_commit_message
        description: Custom merge commit message
      - in: path
        name: merge_request_id
      - in: formData
        name: merge_when_build_succeeds
        description: When true, this merge request will be merged when the pipeline
          succeeds
      - in: formData
        name: sha
        description: When present, must have the HEAD SHA of the source branch
      - in: formData
        name: should_remove_source_branch
        description: When true, the source branch will be deleted if possible
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Merge
      - Request
      - Merge
  /v3/projects/{id}/merge_request/{merge_request_id}/cancel_merge_when_build_succeeds:
    post:
      summary: Post Projects Merge Request Merge Request Cancel Merge When Build Succeeds
      description: Post projects merge request merge request cancel merge when build
        succeeds.
      operationId: postV3ProjectsIdMergeRequestMergeRequestIdCancelMergeWhenBuildSucceeds
      x-api-path-slug: v3projectsidmerge-requestmerge-request-idcancel-merge-when-build-succeeds-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Merge
      - Request
      - Cancel
      - Merge
      - When
      - Build
      - Succeeds
  /v3/projects/{id}/merge_request/{merge_request_id}/comments:
    get:
      summary: Get Projects Merge Request Merge Request Comments
      description: Get projects merge request merge request comments.
      operationId: getV3ProjectsIdMergeRequestMergeRequestIdComments
      x-api-path-slug: v3projectsidmerge-requestmerge-request-idcomments-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Merge
      - Request
      - Comments
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