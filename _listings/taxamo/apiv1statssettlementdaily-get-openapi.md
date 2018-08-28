---
swagger: "2.0"
x-collection-name: Taxamo
x-complete: 0
info:
  title: Taxamo Settlement Stats Over Time
  description: Settlement stats over time.
  version: "1"
host: api.taxamo.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/stats/settlement/daily:
    get:
      summary: Settlement Stats Over Time
      description: Settlement stats over time.
      operationId: getDailySettlementStats
      x-api-path-slug: apiv1statssettlementdaily-get
      parameters:
      - in: query
        name: date_from
        description: Date from in yyyy-MM format
      - in: query
        name: date_to
        description: Date to in yyyy-MM format
      - in: query
        name: interval
        description: Interval type - day, week, month
      responses:
        200:
          description: OK
      tags:
      - Settlement
      - Stats
      - Over
      - Time
  /api/v1/stats/transactions:
    get:
      summary: Transaction Stats
      description: Transaction stats.
      operationId: getTransactionsStats
      x-api-path-slug: apiv1statstransactions-get
      parameters:
      - in: query
        name: date_from
        description: Date from in yyyy-MM format
      - in: query
        name: date_to
        description: Date to in yyyy-MM format
      - in: query
        name: interval
        description: Interval
      responses:
        200:
          description: OK
      tags:
      - Transaction
      - Stats
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