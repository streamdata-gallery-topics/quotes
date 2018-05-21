---
swagger: "2.0"
x-collection-name: IEX
x-complete: 1
info:
  title: IEX
  description: the-iex-api-is-a-set-of-services-designed-for-developers-and-engineers-it-can-be-used-to-build-highquality-apps-and-services-were-always-working-to-improve-the-iex-api-please-check-back-for-enhancements-and-improvements
  termsOfService: https://iextrading.com/api-terms/
  version: 1.0.0
host: api.iextrading.com
basePath: /1.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /stock/market/batch:
    get:
      summary: Batch Requests
      description: Returns batch stock quotes.
      operationId: batch-requests
      x-api-path-slug: stockmarketbatch-get
      parameters:
      - ~
      - in: query
        name: range
        description: ' Optional  Used to specify a chart range if chart is used in
          types parameter'
      - in: query
        name: symbols
        description: ' Optional  Comma delimited list of symbols limited to 100'
      - in: query
        name: types
        description: ' Required  Comma delimited list of endpoints to call'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Quotes
      - Batch
  /stock/{symbol}/delayed-quote:
    get:
      summary: Delayed Quote
      description: This returns the 15 minute delayed market quote.
      operationId: delayed-quote
      x-api-path-slug: stocksymboldelayedquote-get
      parameters:
      - in: path
        name: symbol
        description: Stock ticker symbol
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Quotes
  /stock/{symbol}/list:
    get:
      summary: List
      description: Refer to the quote section.
      operationId: list
      x-api-path-slug: stocksymbollist-get
      parameters:
      - in: query
        name: displayPercent
        description: ' Optional  If set to true, all percentage values will be multiplied
          by a factor of 100 (Ex: /stock/aapl/quote?displayPercent=true)'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Quotes
  /stock/{symbol}/previous:
    get:
      summary: Previous
      description: This returns previous day adjusted price data for a single stock,
        or an object keyed by symbol of price data for the whole market.
      operationId: previous
      x-api-path-slug: stocksymbolprevious-get
      parameters:
      - in: path
        name: symbol
        description: Stock ticker symbol
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Quotes
      - Adjustments
  /stock/{symbol}/quote:
    get:
      summary: Quote
      description: Pulls a stock quote using any ticker symbol.
      operationId: quote
      x-api-path-slug: stocksymbolquote-get
      parameters:
      - in: query
        name: displayPercent
        description: ' Optional If set to true, all percentage values will be multiplied
          by a factor of 100 (Ex: /stock/aapl/quote?displayPercent=true)'
      - in: path
        name: symbol
        description: Stock ticker symbol
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Quotes
  /stock/{symbol}/splits/{range}:
    get:
      summary: Splits
      description: Returns stock splits for any date range using ticker symbol.
      operationId: splits
      x-api-path-slug: stocksymbolsplitsrange-get
      parameters:
      - in: path
        name: range
        description: The date range
        type: string
        format: string
      - in: path
        name: symbol
        description: Stock ticker symbol
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Quotes
      - Splits
---