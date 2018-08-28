swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
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