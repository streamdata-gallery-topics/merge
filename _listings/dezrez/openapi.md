---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/branch/createscheduledmailmerge:
    post:
      summary: Save a scheduled mail merge.
      description: Save a scheduled mail merge..
      operationId: Branch_CreateScheduledMailMergeByscheduledMailMerge
      x-api-path-slug: apibranchcreatescheduledmailmerge-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: scheduledMailMerge
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Save
      - Scheduled
      - Mail
      - Merge
  /api/documentgeneration/updatelettertemplate/{id}:
    post:
      summary: Updates a merge letter template
      description: Updates a merge letter template.
      operationId: DocumentGeneration_UpdateLetterTemplateByidByletterTemplate
      x-api-path-slug: apidocumentgenerationupdatelettertemplateid-post
      parameters:
      - in: path
        name: id
        description: Document Id for the template
      - in: body
        name: letterTemplate
        description: The letter template
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Merge
      - Letter
      - Template
  /api/documentgeneration/searchmergefields:
    get:
      summary: Search Merge Fields
      description: Search merge fields.
      operationId: DocumentGeneration_SearchMergeFieldsBypartialName
      x-api-path-slug: apidocumentgenerationsearchmergefields-get
      parameters:
      - in: query
        name: partialName
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Search
      - Merge
      - Fields
  /api/stationary/html/{brandId}:
    get:
      summary: "Does a simple merge of the selected envelopeTemplatePack using the
        data supplied\r\nwill only use certain merge functions, and the correspondence
        can only contain one envelope and the envelope can only contain one document."
      description: "Does a simple merge of the selected envelopetemplatepack using
        the data supplied\r\nwill only use certain merge functions, and the correspondence
        can only contain one envelope and the envelope can only contain one document.."
      operationId: Stationary_HtmlStationaryBybrandId
      x-api-path-slug: apistationaryhtmlbrandid-get
      parameters:
      - in: path
        name: brandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Does
      - Simple
      - Merge
      - Of
      - Selected
      - EnvelopeTemplatePack
      - Using
      - Data
      - "Supplied\r\nWill"
      - Only
      - Use
      - Certain
      - Merge
      - Functions
      - ""
      - Correspondence
      - Can
      - Only
      - Contain
      - Envelope
      - Envelope
      - Can
      - Only
      - Contain
      - Document
  /api/stationary/sms/{brandId}:
    get:
      summary: "Does a simple merge of the selected envelopeTemplatePack using the
        data supplied\r\nwill only use certain merge functions, and the correspondence
        can only contain one envelope and the envelope can only contain one document."
      description: "Does a simple merge of the selected envelopetemplatepack using
        the data supplied\r\nwill only use certain merge functions, and the correspondence
        can only contain one envelope and the envelope can only contain one document.."
      operationId: Stationary_SmsStationaryBybrandId
      x-api-path-slug: apistationarysmsbrandid-get
      parameters:
      - in: path
        name: brandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Does
      - Simple
      - Merge
      - Of
      - Selected
      - EnvelopeTemplatePack
      - Using
      - Data
      - "Supplied\r\nWill"
      - Only
      - Use
      - Certain
      - Merge
      - Functions
      - ""
      - Correspondence
      - Can
      - Only
      - Contain
      - Envelope
      - Envelope
      - Can
      - Only
      - Contain
      - Document
  /api/admin/system/updateDocumentGenerationMetadataFile:
    post:
      summary: Updates the metadata for document generation merge fields
      description: Updates the metadata for document generation merge fields.
      operationId: System_UpdateDocumentGenerationMetadataFile
      x-api-path-slug: apiadminsystemupdatedocumentgenerationmetadatafile-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Metadatadocument
      - Generation
      - Merge
      - Fields
---