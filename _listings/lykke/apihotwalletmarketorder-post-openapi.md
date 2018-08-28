---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Add API Hotwallet Marketorder
  version: 1.0.0
  description: Add api hotwallet marketorder.
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/Market/converter/tobase:
    post:
      summary: Add API Market Converter Tobase
      description: Add api market converter tobase.
      operationId: ApiMarketConverterTobasePost
      x-api-path-slug: apimarketconvertertobase-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market
      - Converter
      - Tobase
  /api/HotWallet/marketOrder:
    post:
      summary: Add API Hotwallet Marketorder
      description: Add api hotwallet marketorder.
      operationId: MarketOrder
      x-api-path-slug: apihotwalletmarketorder-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SignatureVerificationToken
        description: signature verification token
      responses:
        200:
          description: OK
      tags:
      - Hotwallet
      - Marketorder
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