---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Super Quotes Get Quotes
  description: Returns quotes for given securities.
  version: 1.0.0
host: superquotes.xignite.com
basePath: xSuperQuotes.json/XigniteSuperQuotes
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetQuotes:
    get:
      summary: Get Quotes
      description: Returns quotes for given securities.
      operationId: GetQuotes
      x-api-path-slug: getquotes-get
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
      - Quotes
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