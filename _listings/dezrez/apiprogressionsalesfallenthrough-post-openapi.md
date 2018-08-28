---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Set Marketing Role as Fallen Through
  version: 1.0.0
  description: Set marketing role as fallen through.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/documentgeneration/recreatepropertymarketreport/{propertyId}:
    post:
      summary: Creates a new Property Market Report document.
      description: Creates a new property market report document..
      operationId: DocumentGeneration_RecreatePropertyMarketReportBypropertyId
      x-api-path-slug: apidocumentgenerationrecreatepropertymarketreportpropertyid-post
      parameters:
      - in: path
        name: propertyId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Property
      - Market
      - Report
      - Document
  /api/progression/lettings/fallenthrough:
    post:
      summary: Set Marketing Role as Fallen Through
      description: Set marketing role as fallen through.
      operationId: LettingsProgression_FallenThroughByfallenThroughDataContract
      x-api-path-slug: apiprogressionlettingsfallenthrough-post
      parameters:
      - in: body
        name: fallenThroughDataContract
        description: Details of the fallen though
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Marketing
      - Role
      - As
      - Fallen
      - Through
  /api/progression/sales/fallenthrough:
    post:
      summary: Set Marketing Role as Fallen Through
      description: Set marketing role as fallen through.
      operationId: SalesProgression_FallenThroughByfallenThroughDataContract
      x-api-path-slug: apiprogressionsalesfallenthrough-post
      parameters:
      - in: body
        name: fallenThroughDataContract
        description: Details of the fallen though
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Marketing
      - Role
      - As
      - Fallen
      - Through
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