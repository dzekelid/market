---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Delete a property market reference
  description: Deletes a property market reference. The ID of the property and the
    ID of the market must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/items/attributes/{attributeId}/value_market_names:
    get:
      summary: Search attribute value market names
      description: Search attribute value market names.
      operationId: getRestItemsAttributesAttributeValueMarketNames
      x-api-path-slug: restitemsattributesattributeidvalue-market-names-get
      parameters:
      - in: path
        name: attributeId
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: lang
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: referenceType
      responses:
        200:
          description: OK
      tags:
      - Search
      - Attribute
      - Value
      - Market
      - Names
    post:
      summary: Create an attribute value market name
      description: Creates an attribute value market name.
      operationId: postRestItemsAttributesAttributeValueMarketNames
      x-api-path-slug: restitemsattributesattributeidvalue-market-names-post
      parameters:
      - in: body
        name: /rest/items/attributes/{attributeId}/value_market_names
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: attributeId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Market
      - Name
  /rest/items/attributes/{attributeId}/value_market_names/{valueId}/{lang}/{referenceType}:
    delete:
      summary: Delete an attribute value market name
      description: Deletes an attribute value market name. The attribute value ID
        and language must be specified.
      operationId: deleteRestItemsAttributesAttributeValueMarketNamesValueLangReferencetype
      x-api-path-slug: restitemsattributesattributeidvalue-market-namesvalueidlangreferencetype-delete
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: lang
      - in: path
        name: referenceType
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Market
      - Name
    put:
      summary: Update an attribute value market name
      description: Updates an attribute value market name. The attribute value ID
        and language must be specified.
      operationId: putRestItemsAttributesAttributeValueMarketNamesValueLangReferencetype
      x-api-path-slug: restitemsattributesattributeidvalue-market-namesvalueidlangreferencetype-put
      parameters:
      - in: body
        name: /rest/items/attributes/{attributeId}/value_market_names/{valueId}/{lang}/{referenceType}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: attributeId
      - in: path
        name: lang
      - in: path
        name: referenceType
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Market
      - Name
  /rest/items/properties/{id}/market_references:
    get:
      summary: List property market references
      description: Lists the property market references of a property. The ID of the
        property must be specified.
      operationId: getRestItemsPropertiesMarketReferences
      x-api-path-slug: restitemspropertiesidmarket-references-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Market
      - References
    post:
      summary: Create a property market reference
      description: Creates a property market reference.
      operationId: postRestItemsPropertiesMarketReferences
      x-api-path-slug: restitemspropertiesidmarket-references-post
      parameters:
      - in: body
        name: /rest/items/properties/{id}/market_references
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Market
      - Reference
  /rest/items/properties/{id}/market_references/{marketId}:
    delete:
      summary: Delete a property market reference
      description: Deletes a property market reference. The ID of the property and
        the ID of the market must be specified.
      operationId: deleteRestItemsPropertiesMarketReferencesMarket
      x-api-path-slug: restitemspropertiesidmarket-referencesmarketid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: marketId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Market
      - Reference
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