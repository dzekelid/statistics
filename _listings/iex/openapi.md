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
---