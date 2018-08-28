---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Create new listing market
  description: |-
    Creates a new listing market. Based on the given options this call can create multiple listing markets. If the
    'optionTemplateId' parameter is provided and the listing option template includes options for different markets
    than one listing market will be created for each market.
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
    get:
      summary: Get a property market reference
      description: Gets a property market reference. The market ID and the property
        ID must be specified.
      operationId: getRestItemsPropertiesMarketReferencesMarket
      x-api-path-slug: restitemspropertiesidmarket-referencesmarketid-get
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
    put:
      summary: Update a property market reference
      description: Updates a property market reference.
      operationId: putRestItemsPropertiesMarketReferencesMarket
      x-api-path-slug: restitemspropertiesidmarket-referencesmarketid-put
      parameters:
      - in: body
        name: /rest/items/properties/{id}/market_references/{marketId}
        schema:
          $ref: '#/definitions/holder'
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
  /rest/items/{id}/variations/{variationId}/market_ident_numbers:
    post:
      summary: Create a market ident number
      description: Creates a market ident number (ASIN/ePID) for a variation.
      operationId: postRestItemsVariationsVariationMarketEntNumbers
      x-api-path-slug: restitemsidvariationsvariationidmarket-ident-numbers-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/market_ident_numbers
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Market
      - Ident
      - Number
  /rest/items/{id}/variations/{variationId}/market_ident_numbers/{marketIdentNumberId}:
    delete:
      summary: Deletes a market ident number
      description: Deletes a market ident number (ASIN/ePID) of a variation.
      operationId: deleteRestItemsVariationsVariationMarketEntNumbersMarketentnumber
      x-api-path-slug: restitemsidvariationsvariationidmarket-ident-numbersmarketidentnumberid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: marketIdentNumberId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - S
      - Market
      - Ident
      - Number
    get:
      summary: Get a market ident number
      description: Gets a market ident number (ASIN/ePID) of a variation.
      operationId: getRestItemsVariationsVariationMarketEntNumbersMarketentnumber
      x-api-path-slug: restitemsidvariationsvariationidmarket-ident-numbersmarketidentnumberid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: marketIdentNumberId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Market
      - Ident
      - Number
    put:
      summary: Updates a market ident number
      description: Updates a market ident number (ASIN/ePID) of a variation.
      operationId: putRestItemsVariationsVariationMarketEntNumbersMarketentnumber
      x-api-path-slug: restitemsidvariationsvariationidmarket-ident-numbersmarketidentnumberid-put
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/market_ident_numbers/{marketIdentNumberId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: marketIdentNumberId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - S
      - Market
      - Ident
      - Number
  /rest/items/{id}/variations/{variationId}/variation_markets:
    delete:
      summary: Delete all market links of one variation
      description: Deletes all links of one variation. The ID of the variation must
        be specified.
      operationId: deleteRestItemsVariationsVariationVariationMarkets
      x-api-path-slug: restitemsidvariationsvariationidvariation-markets-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Market
      - Links
      - Of
      - Variation
    post:
      summary: Create link between variation and market
      description: Creates a link between a variation and a market. The ID of the
        item, the ID of the variation and the ID of the market must be specified.
      operationId: postRestItemsVariationsVariationVariationMarkets
      x-api-path-slug: restitemsidvariationsvariationidvariation-markets-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_markets
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Market
  /rest/items/{id}/variations/{variationId}/variation_markets/{marketplaceId}:
    delete:
      summary: Delete link between variation and market
      description: Deletes a link between a variation and a market. The ID of the
        item, the ID of the variation and the ID of the market must be specified.
      operationId: deleteRestItemsVariationsVariationVariationMarketsMarketplace
      x-api-path-slug: restitemsidvariationsvariationidvariation-marketsmarketplaceid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: marketplaceId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Market
  /rest/listings/markets:
    post:
      summary: Create new listing market
      description: |-
        Creates a new listing market. Based on the given options this call can create multiple listing markets. If the
        'optionTemplateId' parameter is provided and the listing option template includes options for different markets
        than one listing market will be created for each market.
      operationId: postRestListingsMarkets
      x-api-path-slug: restlistingsmarkets-post
      parameters:
      - in: body
        name: /rest/listings/markets
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Listing
      - Market
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