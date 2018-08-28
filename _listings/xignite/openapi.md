swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite VWAP
  description: provides-delayed-and-historical-volumeweightedaverage-price-vwap-information-
  version: 1.0.0
host: www.xignite.com
basePath: xVWAP.json/XigniteVWAP
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetMarketNewsDetails:
    get:
      summary: Get Market News Details
      description: Returns the summary content for a specified headline.
      operationId: GetMarketNewsDetails
      x-api-path-slug: getmarketnewsdetails-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Market
      - News
      - Details
  /GetTodaysMarketHeadlines:
    get:
      summary: Get Todays Market Headlines
      description: Returns all market headlines that were published today.
      operationId: GetTodaysMarketHeadlines
      x-api-path-slug: gettodaysmarketheadlines-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Todays
      - Market
      - Headlines
  /GetTopMarketHeadlines:
    get:
      summary: Get Top Market Headlines
      description: Returns the most recent specified number of market headlines.
      operationId: GetTopMarketHeadlines
      x-api-path-slug: gettopmarketheadlines-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Top
      - Market
      - Headlines
  /GetTopMarketHeadlinesBySector:
    get:
      summary: Get Top Market Headlines By Sector
      description: Returns the most recent specified number of market headlines associated
        with a specified sector.
      operationId: GetTopMarketHeadlinesBySector
      x-api-path-slug: gettopmarketheadlinesbysector-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Top
      - Market
      - Headlines
      - Sector
  /GetTodaysMarketReleases:
    get:
      summary: Get Todays Market Releases
      description: Return press releases for today.
      operationId: GetTodaysMarketReleases
      x-api-path-slug: gettodaysmarketreleases-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Todays
      - Market
      - Releases
  /GetTodaysMarketHeadlinesBySector:
    get:
      summary: Get Todays Market Headlines By Sector
      description: Returns all market headlines that were published today for a specified
        sector.
      operationId: GetTodaysMarketHeadlinesBySector
      x-api-path-slug: gettodaysmarketheadlinesbysector-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Todays
      - Market
      - Headlines
      - Sector
  /GetHistoricalMarketHeadlines:
    get:
      summary: Get Historical Market Headlines
      description: Returns all market headlines that were published in a specified
        time frame.
      operationId: GetHistoricalMarketHeadlines
      x-api-path-slug: gethistoricalmarketheadlines-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Market
      - Headlines
  /GetHistoricalMarketHeadlinesBySector:
    get:
      summary: Get Historical Market Headlines By Sector
      description: Returns all market headlines that were published in a specified
        time frame for a specified sector.
      operationId: GetHistoricalMarketHeadlinesBySector
      x-api-path-slug: gethistoricalmarketheadlinesbysector-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Market
      - Headlines
      - Sector
  /GetTopMarketSummaries:
    get:
      summary: Get Top Market Summaries
      description: Return the top market summaries.
      operationId: GetTopMarketSummaries
      x-api-path-slug: gettopmarketsummaries-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Top
      - Market
      - Summaries
  /GetTopMoversByMarketCapitalization:
    get:
      summary: Get Top Movers By Market Capitalization
      description: This operation returns quote information about the top moving equities
        filtered by market capitalization from NYSE, NASDAQ and AMEX.
      operationId: postGettopmoversbymarketcapitalization
      x-api-path-slug: gettopmoversbymarketcapitalization-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Top
      - Movers
      - Market
      - Capitalization
  /GetTopGainersByMarketCapitalization:
    get:
      summary: Get Top Gainers By Market Capitalization
      description: This operation returns quote information about the top gaining
        equities filtered by market capitalization from NYSE, NASDAQ and AMEX.
      operationId: postGettopgainersbymarketcapitalization
      x-api-path-slug: gettopgainersbymarketcapitalization-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Top
      - Gainers
      - Market
      - Capitalization
  /GetTopLosersByMarketCapitalization:
    get:
      summary: Get Top Losers By Market Capitalization
      description: This operation returns quote information about the top losing equities
        filtered by market capitalization from NYSE, NASDAQ and AMEX.
      operationId: postGettoplosersbymarketcapitalization
      x-api-path-slug: gettoplosersbymarketcapitalization-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Top
      - Losers
      - Market
      - Capitalization
  GetHistoricalMarketHeadlines/:
    get:
      summary: Get Historical Market Headlines
      description: Returns market headlines for a date range.
      operationId: getGethistoricalmarketheadlines
      x-api-path-slug: gethistoricalmarketheadlines-get
      parameters:
      - in: query
        name: EndDate
        description: The end date range
      - in: query
        name: Source
        description: The source of the news
      - in: query
        name: StartDate
        description: The start date range
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Market
      - Headlines
  GetLastMarketHeadlines/:
    get:
      summary: Get Last Market Headlines
      description: Returns market headlines published since a specific date and time.
      operationId: getGetlastmarketheadlines
      x-api-path-slug: getlastmarketheadlines-get
      parameters:
      - in: query
        name: SinceDate
        description: The beginning of data range
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Last
      - Market
      - Headlines
  GetTopMarketHeadlines/:
    get:
      summary: Get Top Market Headlines
      description: Returns a given number of market headlines published most recently.
      operationId: getGettopmarketheadlines
      x-api-path-slug: gettopmarketheadlines-get
      parameters:
      - in: query
        name: Count
        description: The number of news items to return
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Top
      - Market
      - Headlines
  SearchMarketHeadlines/:
    get:
      summary: Search Market Headlines
      description: Search market headlines across all companies based on date, source,
        and title.
      operationId: getSearchmarketheadlines
      x-api-path-slug: searchmarketheadlines-get
      parameters:
      - in: query
        name: EndDate
        description: The end date range
      - in: query
        name: Source
        description: The source of the news
      - in: query
        name: StartDate
        description: The start date range
      - in: query
        name: Title
        description: Title of the headlines
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Search
      - Market
      - Headlines