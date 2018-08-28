---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Historical Get Historical Statistics
  description: Returns Historical statistics for a security. For more information,
    go to http://www.xignite.com/
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
  /GetGlobalHistoricalStatistics:
    get:
      summary: Get Global Historical Statistics
      description: Returns Global Historical statistics for a security. For more information,
        go to http://www.xignite.com/
      operationId: postGetglobalhistoricalstatistics
      x-api-path-slug: getglobalhistoricalstatistics-get
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
      - Global
      - Historical
      - Statistics
  /GetMasterStatisticsByExchange:
    get:
      summary: Get Master Statistics By Exchange
      description: Get statistical information about exchanges.
      operationId: GetMasterStatisticsByExchange
      x-api-path-slug: getmasterstatisticsbyexchange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Statistics
      - Exchange
  /GetHistoricalStatistics:
    get:
      summary: Get Historical Statistics
      description: Returns Historical statistics for a security. For more information,
        go to http://www.xignite.com/
      operationId: postGethistoricalstatistics
      x-api-path-slug: gethistoricalstatistics-get
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
      - Statistics
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