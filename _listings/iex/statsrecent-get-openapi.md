---
swagger: "2.0"
x-collection-name: IEX
x-complete: 0
info:
  title: IEX Trading API Recent
  description: This call will return a minimum of the last five trading days up to
    all trading days of the current month.
  termsOfService: https://iextrading.com/api-terms/
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: api.iextrading.com
basePath: /1.0
paths:
  /stats/recent:
    get:
      summary: Recent
      description: This call will return a minimum of the last five trading days up
        to all trading days of the current month.
      operationId: recent
      x-api-path-slug: statsrecent-get
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Statistics
x-streamrank:
  polling_total_time_average: "0.16"
  polling_size_download_average: "1555.36"
  streaming_total_time_average: "0.09"
  streaming_size_download_average: "781.12"
  change_yes: "50"
  change_no: "1743"
  time_percentage: "42"
  size_percentage: "50"
  change_percentage: "3"
  last_run: "2018-02-20"
  days_run: "4"
  minute_run: "0"
---