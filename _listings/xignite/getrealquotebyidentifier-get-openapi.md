---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite BATS Real Time Get Real Quote By Identifier
  description: Returns a real-time quote for a security based on the last trade execution.
  version: 1.0.0
host: batsrealtime.xignite.com
basePath: xBATSRealTime.json/XigniteBATSRealTime
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetRealQuotes:
    get:
      summary: Get Real Quotes
      description: Returns a collection of real time stock quotes for a comma-separated
        list of stock quotes.
      operationId: GetRealQuotes
      x-api-path-slug: getrealquotes-get
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
      - Real
      - Quotes
  /GetRealQuotesByIdentifiers:
    get:
      summary: Get Real Quotes By Identifiers
      description: Returns a collection of real time stock quotes for a comma-separated
        list of stock quotes.
      operationId: GetRealQuotesByIdentifiers
      x-api-path-slug: getrealquotesbyidentifiers-get
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
      - Real
      - Quotes
      - Identifiers
  /GetRealQuote:
    get:
      summary: Get Real Quote
      description: Returns real time stock quote for a given stock ticker
      operationId: GetRealQuote
      x-api-path-slug: getrealquote-get
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
      - Real
      - Quote
  /GetRealQuoteByIdentifier:
    get:
      summary: Get Real Quote By Identifier
      description: Returns a real-time quote for a security based on the last trade
        execution.
      operationId: GetRealQuoteByIdentifier
      x-api-path-slug: getrealquotebyidentifier-get
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
      - Real
      - Quote
      - Identifier
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