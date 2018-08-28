---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Create a property market
  description: Creates a property market.
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
  /rest/listings/markets/directories:
    get:
      summary: Get all listing market directories
      description: Gets all listing market directories.
      operationId: getRestListingsMarketsDirectories
      x-api-path-slug: restlistingsmarketsdirectories-get
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Directories
    post:
      summary: Create listing market directory
      description: Creates a listing market directory.
      operationId: postRestListingsMarketsDirectories
      x-api-path-slug: restlistingsmarketsdirectories-post
      parameters:
      - in: body
        name: /rest/listings/markets/directories
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Directory
  /rest/listings/markets/directories/{id}:
    delete:
      summary: Delete listing market directory
      description: Deletes a listing market directory by ID.
      operationId: deleteRestListingsMarketsDirectories
      x-api-path-slug: restlistingsmarketsdirectoriesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Directory
    get:
      summary: Get a listing market directory
      description: Gets a listing market directory by ID.
      operationId: getRestListingsMarketsDirectories
      x-api-path-slug: restlistingsmarketsdirectoriesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Directory
    put:
      summary: Update listing market directory
      description: Updates a listing market directory by ID.
      operationId: putRestListingsMarketsDirectories
      x-api-path-slug: restlistingsmarketsdirectoriesid-put
      parameters:
      - in: body
        name: /rest/listings/markets/directories/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Directory
  /rest/listings/markets/histories:
    get:
      summary: List listing market history
      description: Lists listing market history by filter options.
      operationId: getRestListingsMarketsHistories
      x-api-path-slug: restlistingsmarketshistories-get
      parameters:
      - in: query
        name: credentialsId
        description: Filter that restricts the search result to listing market histories
          with given credential ID
      - in: query
        name: directoryId
        description: Filter that restricts the search result to listing market histories
          with a given directory ID
      - in: query
        name: duration
        description: Filter that restricts the search result to listing market histories
          with given duration
      - in: query
        name: externalId
        description: Filter that restricts the search result to listing market histories
          with given external id
      - in: query
        name: firstPlatformCategoryId
        description: Filter that restricts the search result to listing market histories
          with first platform category ID equal to the given ID
      - in: query
        name: firstShopCategoryId
        description: Filter that restricts the search result to listing market histories
          with first shop category ID equal to the given ID
      - in: query
        name: isClickAndCollect
        description: Filter that restricts the search result to listing market histories
          that belong to eBay Click & Collect
      - in: query
        name: isEbayPlus
        description: Filter that restricts the search result to listing market histories
          that belong to eBay Plus
      - in: query
        name: itemId
        description: Filter that restricts the search result to listing market histories
          that belong to a given item ID
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: lastSale
        description: Filter that restricts the search result to listing market histories
          with last sale before given date
      - in: query
        name: listingId
        description: Filter that restricts the search result to listing market histories
          that belong to a given listing ID
      - in: query
        name: listingMarketId
        description: Filter that restricts the search result to listing market histories
          that match the given listing market ID(s)
      - in: query
        name: listingTypeId
        description: Filter that restricts the search result to listing market histories
          that belong to a listing of a custom type ID
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: referrerId
        description: Filter that restricts the search result to listing market histories
          with given referrer ID
      - in: query
        name: secondPlatformCategoryId
        description: Filter that restricts the search result to listing market histories
          with second platform category ID equal to the given ID
      - in: query
        name: secondShopCategoryId
        description: Filter that restricts the search result to listing market histories
          with second shop category ID equal to the given ID
      - in: query
        name: shippingProfileId
        description: Filter that restricts the search result to listing market histories
          that belong to a given shipping profile
      - in: query
        name: statusId
        description: Filter that restricts the search result to listing market histories
          with a custom status status ID
      - in: query
        name: stockCondition
        description: Filter that restricts the search result to listing market histories
          with a custom stock condition
      - in: query
        name: stockDependenceTypeId
        description: Filter that restricts the search result to listing market histories
          that belong to a listing with a custom stock dependence type ID
      - in: query
        name: textData
        description: Filter that restricts the search result to listing market histories
          that match given text in listing title or description
      - in: query
        name: thirdShopCategoryId
        description: Filter that restricts the search result to listing market histories
          with third shop category ID equal to the given ID
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to listing market histories
          that were last updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to listing market histories
          that were last updated within a specified period of time
      - in: query
        name: variationId
        description: Filter that restricts the search result to listing market histories
          that match the given variation ID(s)
      - in: query
        name: variations
        description: Filter that restricts the search result to listing market histories
          with a custom variation condition
      - in: query
        name: verified
        description: Filter that restricts the search result to listing market histories
          that are verified
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Market
      - History
  /rest/listings/markets/histories/update/{id?}:
    put:
      summary: Update listing market histories
      description: |-
        Updates listing market histories by given update options. The listing market histories are not directly revised,
        they are added to the batch processing lists, waiting to be revised by automated background processes.
      operationId: putRestListingsMarketsHistoriesUpdate
      x-api-path-slug: restlistingsmarketshistoriesupdateid-put
      parameters:
      - in: query
        name: id
        description: The ID of the listing market history that needs to be ended
      - in: path
        name: id?
      - in: query
        name: options
        description: Multiple update options
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Histories
  /rest/listings/markets/histories/{id}:
    get:
      summary: Get a listing market history
      description: Gets a listing market history by given ID.
      operationId: getRestListingsMarketsHistories
      x-api-path-slug: restlistingsmarketshistoriesid-get
      parameters:
      - in: path
        name: id
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - History
  /rest/listings/markets/infos:
    get:
      summary: Search listing market info
      description: Search listing market info by filter options.
      operationId: getRestListingsMarketsInfos
      x-api-path-slug: restlistingsmarketsinfos-get
      parameters:
      - in: query
        name: code
        description: Filter that restricts the search result to listing market info
          with given codes
      - in: query
        name: createdAtFrom
        description: Filter that restricts the search result to listing markets that
          were last updated on the specified date
      - in: query
        name: createdAtTo
        description: Filter that restricts the search result to listing markets that
          were last updated within a specified period of time
      - in: query
        name: id
        description: Filter that restricts the search result to listing market info
          that match the given ID(s)
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: listingMarketId
        description: Filter that restricts the search result to listing market info
          that match the given listing market ID(s)
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: type
        description: Filter that restricts the search result to listing market info
          with a custom type
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Search
      - Listing
      - Market
      - Info
  /rest/listings/markets/start/{id?}:
    post:
      summary: Start the market listing on the designated market.
      description: Starts the market listing on the designated markets.
      operationId: postRestListingsMarketsStart
      x-api-path-slug: restlistingsmarketsstartid-post
      parameters:
      - in: query
        name: distribution
        description: The number of minutes that the listing should be started
      - in: query
        name: id
        description: The ID of the listing market that needs to be started
      - in: path
        name: id?
      - in: query
        name: startAt
        description: When should the listings be started
      responses:
        200:
          description: OK
      tags:
      - Start
      - Market
      - Listing
      - "On"
      - Designated
      - Market
  /rest/listings/markets/texts:
    get:
      summary: List listing market texts
      description: Lists listing market texts by filter options.
      operationId: getRestListingsMarketsTexts
      x-api-path-slug: restlistingsmarketstexts-get
      parameters:
      - in: query
        name: contains
        description: Filter that restricts the search result to listing market texts
          which title, subtitle or description contain the given value
      - in: query
        name: id
        description: Filter that restricts the search result to listing market texts
          with specific ID
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: language
        description: Filter that restricts the search result to listing market texts
          for a specific language
      - in: query
        name: listingMarketId
        description: Filter that restricts the search result to listing market texts
          with specific listing market IDs
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Market
      - Texts
    post:
      summary: Create a listing market text
      description: Creates a listing market text for a given listing market ID. If
        an entry with same data already exists the request will be ignored and the
        old entry will be returned.
      operationId: postRestListingsMarketsTexts
      x-api-path-slug: restlistingsmarketstexts-post
      parameters:
      - in: body
        name: /rest/listings/markets/texts
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: listingMarketId
        description: The listing market ID this text belongs to
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Text
  /rest/listings/markets/texts/{id}:
    delete:
      summary: Delete a listing market text
      description: Deletes a listing market text for a given listing market text ID.
      operationId: deleteRestListingsMarketsTexts
      x-api-path-slug: restlistingsmarketstextsid-delete
      parameters:
      - in: path
        name: id
      - in: query
        name: lang
        description: The listing market text language that should be updated
      - in: query
        name: listingMarketId
        description: The listing market ID this text belongs to
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Text
    get:
      summary: Get a listing market text
      description: Gets a listing market text by providing its ID.
      operationId: getRestListingsMarketsTexts
      x-api-path-slug: restlistingsmarketstextsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Text
  /rest/listings/markets/texts/{listingMarketId}/{lang}:
    put:
      summary: Update a listing market text
      description: Updates a listing market text for a given listing market ID and
        language.
      operationId: putRestListingsMarketsTextsListingmarketLang
      x-api-path-slug: restlistingsmarketstextslistingmarketidlang-put
      parameters:
      - in: body
        name: /rest/listings/markets/texts/{listingMarketId}/{lang}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lang
      - in: path
        name: listingMarketId
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Text
  /rest/listings/markets/{id}:
    delete:
      summary: Delete listing market
      description: Deletes a listing market by ID.
      operationId: deleteRestListingsMarkets
      x-api-path-slug: restlistingsmarketsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
    get:
      summary: Get a listing market
      description: Gets a listing market by given ID.
      operationId: getRestListingsMarkets
      x-api-path-slug: restlistingsmarketsid-get
      parameters:
      - in: path
        name: id
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
    put:
      summary: Update a listing market
      description: Updates a listing market by ID.
      operationId: putRestListingsMarkets
      x-api-path-slug: restlistingsmarketsid-put
      parameters:
      - in: body
        name: /rest/listings/markets/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: query
        name: referrerId
        description: The referrer ID
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
  /rest/markets/settings:
    get:
      summary: List market settings
      description: Lists market settings. The marketplace ID and the type must be
        specified.
      operationId: getRestMarketsSettings
      x-api-path-slug: restmarketssettings-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Market
      - Settings
    post:
      summary: Create market settings
      description: Creates new market settings by given data. The marketplace ID and
        the type must be specified.
      operationId: postRestMarketsSettings
      x-api-path-slug: restmarketssettings-post
      responses:
        200:
          description: OK
      tags:
      - Market
      - Settings
  /rest/markets/settings/bulk:
    post:
      summary: Create market settings
      description: Creates new market settings by given data. The marketplace ID and
        the type must be specified.
      operationId: postRestMarketsSettingsBulk
      x-api-path-slug: restmarketssettingsbulk-post
      responses:
        200:
          description: OK
      tags:
      - Market
      - Settings
    put:
      summary: Update market settings
      description: Updates market settings. The market settings ID must be specified.
      operationId: putRestMarketsSettingsBulk
      x-api-path-slug: restmarketssettingsbulk-put
      responses:
        200:
          description: OK
      tags:
      - Market
      - Settings
  /rest/markets/settings/{settingId}:
    delete:
      summary: Delete market settings
      description: Deletes market settings. The market settings ID must be specified.
      operationId: deleteRestMarketsSettingsSetting
      x-api-path-slug: restmarketssettingssettingid-delete
      parameters:
      - in: path
        name: settingId
      responses:
        200:
          description: OK
      tags:
      - Market
      - Settings
    get:
      summary: Get market settings
      description: Gets market settings. The market settings ID must be specified.
      operationId: getRestMarketsSettingsSetting
      x-api-path-slug: restmarketssettingssettingid-get
      parameters:
      - in: path
        name: settingId
      responses:
        200:
          description: OK
      tags:
      - Market
      - Settings
    put:
      summary: Update market settings
      description: Updates market settings. The market settings ID must be specified.
      operationId: putRestMarketsSettingsSetting
      x-api-path-slug: restmarketssettingssettingid-put
      parameters:
      - in: path
        name: settingId
      responses:
        200:
          description: OK
      tags:
      - Market
      - Settings
  /rest/properties/markets:
    post:
      summary: Create a property market
      description: Creates a property market.
      operationId: postRestPropertiesMarkets
      x-api-path-slug: restpropertiesmarkets-post
      parameters:
      - in: body
        name: /rest/properties/markets
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: propertyId
        description: Property id
      - in: query
        name: referrerId
        description: The referrer id of the property market
      - in: query
        name: referrerSubId
        description: The referrer sub id of the property market
      - in: query
        name: value
        description: The value of the property market
      responses:
        200:
          description: OK
      tags:
      - Property
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