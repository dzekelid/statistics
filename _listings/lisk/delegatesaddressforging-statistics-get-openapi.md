---
swagger: "2.0"
x-collection-name: Lisk
x-complete: 0
info:
  title: Lisk Requests forging stats by delegate
  description: |-
    By passing an existing delegate address and the desired unix timestamps, you can get its forging statistics within the specified timespan.
    If no timestamps are provided, it will use the timestamps from Lisk epoch to current date.
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /delegates/{address}/forging_statistics:
    get:
      summary: Requests forging stats by delegate
      description: |-
        By passing an existing delegate address and the desired unix timestamps, you can get its forging statistics within the specified timespan.
        If no timestamps are provided, it will use the timestamps from Lisk epoch to current date.
      operationId: getForgingStatistics
      x-api-path-slug: delegatesaddressforging-statistics-get
      parameters:
      - in: path
        name: address
        description: Lisk address of a delegate
      - in: query
        name: fromTimestamp
        description: Starting unix timestamp
      - in: query
        name: toTimestamp
        description: Ending unix timestamp
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Forging
      - Stats
      - By
      - Delegate
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