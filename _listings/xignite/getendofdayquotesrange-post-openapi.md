---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global Historical Get End Of Day Quotes Range
  description: Returns a quote a complete range of stock quotes for a given equity.
    This includes the adjusted price as specified.
  version: 1.0.0
host: www.xignite.com
basePath: xGlobalHistorical.json/XigniteGlobalHistorical
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetEndOfDayQuotes:
    post:
      summary: Get End Of Day Quotes
      description: Returns a quote as of a historical date. This includes the adjusted
        price as specified.
      operationId: postGetendofdayquotes
      x-api-path-slug: getendofdayquotes-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - End
      - Of
      - Day
      - Quotes
  /GetEndOfDayQuotesRange:
    post:
      summary: Get End Of Day Quotes Range
      description: Returns a quote a complete range of stock quotes for a given equity.
        This includes the adjusted price as specified.
      operationId: postGetendofdayquotesrange
      x-api-path-slug: getendofdayquotesrange-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - End
      - Of
      - Day
      - Quotes
      - Range
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