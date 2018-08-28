---
name: CoinMarketCap
x-slug: coinmarketcap
description: Cryptocurrency market cap rankings, charts, and more
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28891-pro-coinmarketcap-com.jpg
x-kinRank: "7"
x-alexaRank: "276"
tags: Market
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/market/master/_listings/coinmarketcap/apis.md
specificationVersion: "0.14"
apis:
- name: CoinMarketCap Professional API Documentation - Get aggregate market metrics
    (latest)
  x-api-slug: v1globalmetricsquoteslatest-get
  description: |-
    Get the latest quote of aggregate market metrics. Use the "convert" option to return market values in multiple fiat and cryptocurrency conversions in the same call.

    **This endpoint is available on the following API plans:**
    - Starter
    - Hobbyist
    - Standard
    - Professional
    - Enterprise

    **Cache / Update frequency:** Every ~5 minutes. This endpoint will be migrated to ~1 minute updates shortly.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28891-pro-coinmarketcap-com.jpg
  humanURL: https://pro.coinmarketcap.com
  baseURL: https://pro-api.coinmarketcap.com//
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/market/master/_listings/coinmarketcap/v1globalmetricsquoteslatest-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/market/master/_listings/coinmarketcap/v1globalmetricsquoteslatest-get-openapi.md
- name: CoinMarketCap Professional API Documentation - Get aggregate market metrics
    (historical)
  x-api-slug: v1globalmetricsquoteshistorical-get
  description: |-
    Get an interval of aggregate 24 hour volume and market cap data globally based on time and interval parameters.

    **Technical Details**
    A historic quote for every "interval" period between your "time_start" and "time_end" will be returned.
    If a "time_start" is not supplied, the "interval" will be applied in reverse from "time_end".
    If "time_end" is not supplied, it defaults to the current time.
    At each "interval" period, the historic quote that is closest in time to the requested time will be returned.
    If no historic quotes are available in a given "interval" period up until the next interval period, it will be skipped.

    **Interval Options**
    There are 2 types of time interval formats that may be used for "interval".

    The first are calendar year and time constants in UTC time:
    **"hourly"** - Get the first quote available at the beginning of each calendar hour.
    **"daily"** - Get the first quote available at the beginning of each calendar day.
    **"weekly"** - Get the first quote available at the beginning of each calendar week.
    **"monthly"** - Get the first quote available at the beginning of each calendar month.
    **"yearly"** - Get the first quote available at the beginning of each calendar year.

    The second are relative time intervals.
    **"m"**: Get the first quote available every "m" minutes (60 second intervals). Supported minutes are: "5m", "10m", "15m", "30m", "45m".
    **"h"**: Get the first quote available every "h" hours (3600 second intervals). Supported hour intervals are: "1h", "2h", "3h", "6h", "12h".
    **"d"**: Get the first quote available every "d" days (86400 second intervals). Supported day intervals are: "1d", "2d", "3d", "7d", "14d", "15d", "30d", "60d", "90d", "365d".

    **This endpoint is available on the following API plans:**
    - ~~Starter~~
    - ~~Hobbyist~~
    - Standard (1 month)
    - Professional (12 months)
    - Enterprise (Up to 5 years)

    **Cache / Update frequency:** Every ~5 minutes. This endpoint will be migrated to ~1 minute updates shortly.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28891-pro-coinmarketcap-com.jpg
  humanURL: https://pro.coinmarketcap.com
  baseURL: https://pro-api.coinmarketcap.com//
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/market/master/_listings/coinmarketcap/v1globalmetricsquoteshistorical-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/market/master/_listings/coinmarketcap/v1globalmetricsquoteshistorical-get-openapi.md
- name: CoinMarketCap Professional API Documentation - Get market quotes (latest)
  x-api-slug: v1exchangequoteslatest-get
  description: |-
    Get the latest 24 hour volume quote for 1 or more exchanges. Additional market data fields will be available in the future. Use the "convert" option to return market values in multiple fiat and cryptocurrency conversions in the same call.

    **This endpoint is available on the following API plans:**
    - ~~Starter~~
    - ~~Hobbyist~~
    - Standard
    - Professional
    - Enterprise

    **Cache / Update frequency:** Every ~5 minutes. This endpoint will be migrated to ~1 minute updates shortly.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28891-pro-coinmarketcap-com.jpg
  humanURL: https://pro.coinmarketcap.com
  baseURL: https://pro-api.coinmarketcap.com//
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/market/master/_listings/coinmarketcap/v1exchangequoteslatest-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/market/master/_listings/coinmarketcap/v1exchangequoteslatest-get-openapi.md
- name: CoinMarketCap Professional API Documentation - Get market quotes (historical)
  x-api-slug: v1exchangequoteshistorical-get
  description: |-
    Returns an interval of historic quotes for any exchange based on time and interval parameters.

    Historical exchange quotes currently include:
    volume_24: Combined 24 hour volume for all market pairs at each historical interval.
    num_market_pairs: Number of market pairs available at each historical interval.
    Quotes are returned in USD. Additional currency conversion options and additional fields will be available in the future.

    **Technical Details**
    A historic quote for every "interval" period between your "time_start" and "time_end" will be returned.
    If a "time_start" is not supplied, the "interval" will be applied in reverse from "time_end".
    If "time_end" is not supplied, it defaults to the current time.
    At each "interval" period, the historic quote that is closest in time to the requested time will be returned.
    If no historic quotes are available in a given "interval" period up until the next interval period, it will be skipped.

    **Interval Options**
    There are 2 types of time interval formats that may be used for "interval".

    The first are calendar year and time constants in UTC time:
    **"hourly"** - Get the first quote available at the beginning of each calendar hour.
    **"daily"** - Get the first quote available at the beginning of each calendar day.
    **"weekly"** - Get the first quote available at the beginning of each calendar week.
    **"monthly"** - Get the first quote available at the beginning of each calendar month.
    **"yearly"** - Get the first quote available at the beginning of each calendar year.

    The second are relative time intervals.
    **"m"**: Get the first quote available every "m" minutes (60 second intervals). Supported minutes are: "5m", "10m", "15m", "30m", "45m".
    **"h"**: Get the first quote available every "h" hours (3600 second intervals). Supported hour intervals are: "1h", "2h", "3h", "6h", "12h".
    **"d"**: Get the first quote available every "d" days (86400 second intervals). Supported day intervals are: "1d", "2d", "3d", "7d", "14d", "15d", "30d", "60d", "90d", "365d".

    **This endpoint is available on the following API plans:**
      - ~~Starter~~
      - ~~Hobbyist~~
      - Standard (1 month)
      - Professional (12 months)
      - Enterprise (Up to 5 years)

    **Cache / Update frequency:** Every ~5 minutes. This endpoint will be migrated to ~1 minute updates shortly.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28891-pro-coinmarketcap-com.jpg
  humanURL: https://pro.coinmarketcap.com
  baseURL: https://pro-api.coinmarketcap.com//
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/market/master/_listings/coinmarketcap/v1exchangequoteshistorical-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/market/master/_listings/coinmarketcap/v1exchangequoteshistorical-get-openapi.md
- name: CoinMarketCap Professional API Documentation - List all market pairs (latest)
  x-api-slug: v1exchangemarketpairslatest-get
  description: |-
    Get a list of active market pairs for an exchange. Active means the market pair is open for trading. Use the "convert" option to return market values in multiple fiat and cryptocurrency conversions in the same call.'

      **This endpoint is available on the following API plans:**
      - ~~Starter~~
      - ~~Hobbyist~~
      - Standard
      - Professional
      - Enterprise

    **Cache / Update frequency:** Every ~5 minutes. This endpoint will be migrated to ~1 minute updates shortly.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28891-pro-coinmarketcap-com.jpg
  humanURL: https://pro.coinmarketcap.com
  baseURL: https://pro-api.coinmarketcap.com//
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/market/master/_listings/coinmarketcap/v1exchangemarketpairslatest-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/market/master/_listings/coinmarketcap/v1exchangemarketpairslatest-get-openapi.md
- name: CoinMarketCap Professional API Documentation - Get market quotes (latest)
  x-api-slug: v1cryptocurrencyquoteslatest-get
  description: |-
    Get the latest market quote for 1 or more cryptocurrencies. Use the "convert" option to return market values in multiple fiat and cryptocurrency conversions in the same call.

    **This endpoint is available on the following API plans:**
    - Starter
    - Hobbyist
    - Standard
    - Professional
    - Enterprise

    **Cache / Update frequency:** Every ~1 minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28891-pro-coinmarketcap-com.jpg
  humanURL: https://pro.coinmarketcap.com
  baseURL: https://pro-api.coinmarketcap.com//
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/market/master/_listings/coinmarketcap/v1cryptocurrencyquoteslatest-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/market/master/_listings/coinmarketcap/v1cryptocurrencyquoteslatest-get-openapi.md
- name: CoinMarketCap Professional API Documentation - Get market quotes (historical)
  x-api-slug: v1cryptocurrencyquoteshistorical-get
  description: |-
    Returns an interval of historic market quotes for any cryptocurrency based on time and interval parameters.

    **Technical Details**
    A historic quote for every "interval" period between your "time_start" and "time_end" will be returned.
    If a "time_start" is not supplied, the "interval" will be applied in reverse from "time_end".
    If "time_end" is not supplied, it defaults to the current time.
    At each "interval" period, the historic quote that is closest in time to the requested time will be returned.
    If no historic quotes are available in a given "interval" period up until the next interval period, it will be skipped.

    **Interval Options**
    There are 2 types of time interval formats that may be used for "interval".

    The first are calendar year and time constants in UTC time:
    **"hourly"** - Get the first quote available at the beginning of each calendar hour.
    **"daily"** - Get the first quote available at the beginning of each calendar day.
    **"weekly"** - Get the first quote available at the beginning of each calendar week.
    **"monthly"** - Get the first quote available at the beginning of each calendar month.
    **"yearly"** - Get the first quote available at the beginning of each calendar year.

    The second are relative time intervals.
    **"m"**: Get the first quote available every "m" minutes (60 second intervals). Supported minutes are: "5m", "10m", "15m", "30m", "45m".
    **"h"**: Get the first quote available every "h" hours (3600 second intervals). Supported hour intervals are: "1h", "2h", "3h", "6h", "12h".
    **"d"**: Get the first quote available every "d" days (86400 second intervals). Supported day intervals are: "1d", "2d", "3d", "7d", "14d", "15d", "30d", "60d", "90d", "365d".

    **This endpoint is available on the following API plans:**
    - ~~Starter~~
    - ~~Hobbyist~~
    - Standard (1 month)
    - Professional (12 months)
    - Enterprise (Up to 5 years)

    **Cache / Update frequency:** Every ~5 minutes. This endpoint will be migrated to ~1 minute updates shortly.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28891-pro-coinmarketcap-com.jpg
  humanURL: https://pro.coinmarketcap.com
  baseURL: https://pro-api.coinmarketcap.com//
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/market/master/_listings/coinmarketcap/v1cryptocurrencyquoteshistorical-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/market/master/_listings/coinmarketcap/v1cryptocurrencyquoteshistorical-get-openapi.md
- name: CoinMarketCap Professional API Documentation - Get market pairs (latest)
  x-api-slug: v1cryptocurrencymarketpairslatest-get
  description: |-
    Lists all market pairs for the specified cryptocurrency with associated stats. Use the "convert" option to return market values in multiple fiat and cryptocurrency conversions in the same call.


      **This endpoint is available on the following API plans:**
      - ~~Starter~~
      - ~~Hobbyist~~
      - Standard
      - Professional
      - Enterprise

    **Cache / Update frequency:** Every ~1 minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28891-pro-coinmarketcap-com.jpg
  humanURL: https://pro.coinmarketcap.com
  baseURL: https://pro-api.coinmarketcap.com//
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/market/master/_listings/coinmarketcap/v1cryptocurrencymarketpairslatest-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/market/master/_listings/coinmarketcap/v1cryptocurrencymarketpairslatest-get-openapi.md
x-common:
- type: x-github
  url: https://github.com/coinmarketcap
- type: x-openapi
  url: https://pro-api.coinmarketcap.com/swagger.json
- type: x-api-gallery
  url: http://coinfabrik.api.gallery.streamdata.io
- type: x-email
  url: legal@coinmarketcap.com
- type: x-twitter
  url: https://twitter.com/CoinMarketCap
- type: x-website
  url: https://pro.coinmarketcap.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---