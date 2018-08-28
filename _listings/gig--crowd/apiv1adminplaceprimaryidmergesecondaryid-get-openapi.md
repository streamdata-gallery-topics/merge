---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Get Admin Place Primaryid Merge Secondaryid
  version: 1.0.0
  description: Get admin place primaryid merge secondaryid.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/admin/event/{primaryId}/merge/{secondaryId}:
    get:
      summary: Get Admin Event Primaryid Merge Secondaryid
      description: Get admin event primaryid merge secondaryid.
      operationId: getApiV1AdminEventPrimaryMergeSecondary
      x-api-path-slug: apiv1admineventprimaryidmergesecondaryid-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: primaryId
      - in: path
        name: secondaryId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Primaryid
      - Merge
      - Secondaryid
  /api/v1/admin/place/{primaryId}/merge/{secondaryId}:
    get:
      summary: Get Admin Place Primaryid Merge Secondaryid
      description: Get admin place primaryid merge secondaryid.
      operationId: getApiV1AdminPlacePrimaryMergeSecondary
      x-api-path-slug: apiv1adminplaceprimaryidmergesecondaryid-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: primaryId
      - in: path
        name: secondaryId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Place
      - Primaryid
      - Merge
      - Secondaryid
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