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
  /GetRateStatistics:
    get:
      summary: Get Rate Statistics
      description: Returns statistics for available rates.
      operationId: postGetratestatistics
      x-api-path-slug: getratestatistics-get
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
      - Rate
      - Statistics
  /GetTopicStatistics:
    get:
      summary: Get Topic Statistics
      description: Get statistics for a topic and a period.
      operationId: postGettopicstatistics
      x-api-path-slug: gettopicstatistics-get
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
      - Topic
      - Statistics