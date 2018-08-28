swagger: "2.0"
x-collection-name: Taxamo
x-complete: 1
info:
  title: Taxamo
  description: taxamos-elegant-suite-of-apis-and-comprehensive-reporting-dashboard-enables-digital-merchants-to-easily-comply-with-eu-regulatory-requirements-on-tax-calculation-evidence-collection-tax-return-creation-and-data-storage-
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