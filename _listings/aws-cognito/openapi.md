---
swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 1
info:
  title: AWS Cognito Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=MergeDeveloperIdentities:
    get:
      summary: Merge Developer Identities
      description: |-
        Merges two users having different IdentityIds, existing in the same
                 identity pool, and identified by the same developer provider.
      operationId: mergeDeveloperIdentities
      x-api-path-slug: actionmergedeveloperidentities-get
      parameters:
      - in: query
        name: DestinationUserIdentifier
        description: User identifier for the destination user
        type: string
      - in: query
        name: DeveloperProviderName
        description: The domain by which Cognito will refer to your users
        type: string
      - in: query
        name: IdentityPoolId
        description: An identity pool ID in the format REGION:GUID
        type: string
      - in: query
        name: SourceUserIdentifier
        description: User identifier for the source user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Developer Identities
---