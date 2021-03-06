---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Historical Get Historical Quotes As Of
  description: This operation returns a range of quotes for a security.
  version: 1.0.0
host: www.xignite.com
basePath: xHistorical.json/XigniteHistorical
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetHistoricalQuotesAdjusted:
    post:
      summary: Get Historical Quotes Adjusted
      description: Returns a quote as of a historical date. This includes split and
        dividends adjusted price.
      operationId: postGethistoricalquotesadjusted
      x-api-path-slug: gethistoricalquotesadjusted-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Quotes
      - Adjusted
  /GetHistoricalMonthlyQuotesRangeAdjusted:
    post:
      summary: Get Historical Monthly Quotes Range Adjusted
      description: This operation returns end of month quotes for a US equity. This
        includes split and dividends adjusted price.
      operationId: postGethistoricalmonthlyquotesrangeadjusted
      x-api-path-slug: gethistoricalmonthlyquotesrangeadjusted-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Monthly
      - Quotes
      - Range
      - Adjusted
  /GetHistoricalQuotesAsOfAdjusted:
    post:
      summary: Get Historical Quotes As Of Adjusted
      description: This operation returns a range of quotes for a security. This includes
        split and dividends adjusted price.
      operationId: postGethistoricalquotesasofadjusted
      x-api-path-slug: gethistoricalquotesasofadjusted-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Quotes
      - As
      - Adjusted
  /GetHistoricalQuotesRangeAdjusted:
    post:
      summary: Get Historical Quotes Range Adjusted
      description: This operation returns a complete range of stock quotes for a US
        equity. This includes and dividends adjusted price.
      operationId: postGethistoricalquotesrangeadjusted
      x-api-path-slug: gethistoricalquotesrangeadjusted-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Quotes
      - Range
      - Adjusted
  /GetHistoricalWeeklyQuotesRangeAdjusted:
    post:
      summary: Get Historical Weekly Quotes Range Adjusted
      description: This operation returns end of week quotes for a US equity. This
        includes split and dividends adjusted price.
      operationId: postGethistoricalweeklyquotesrangeadjusted
      x-api-path-slug: gethistoricalweeklyquotesrangeadjusted-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Weekly
      - Quotes
      - Range
      - Adjusted
  /GetHistoricalQuarterlyQuotesRangeAdjusted:
    post:
      summary: Get Historical Quarterly Quotes Range Adjusted
      description: This operation returns end of quarter quotes for a US equity. This
        includes split and dividends adjusted price.
      operationId: postGethistoricalquarterlyquotesrangeadjusted
      x-api-path-slug: gethistoricalquarterlyquotesrangeadjusted-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Quarterly
      - Quotes
      - Range
      - Adjusted
  /GetHistoricalQuotes:
    post:
      summary: Get Historical Quotes
      description: Returns a quote as of a historical date. This includes split adjusted
        price.
      operationId: postGethistoricalquotes
      x-api-path-slug: gethistoricalquotes-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Quotes
  /GetHistoricalQuotesAsOf:
    post:
      summary: Get Historical Quotes As Of
      description: This operation returns a range of quotes for a security.
      operationId: postGethistoricalquotesasof
      x-api-path-slug: gethistoricalquotesasof-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Quotes
      - As
      - Of
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