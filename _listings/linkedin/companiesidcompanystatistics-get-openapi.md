---
swagger: "2.0"
x-collection-name: LinkedIn
x-complete: 0
info:
  title: LinkedIn Get Companies Company Statistics
  description: Get companies  company statistics
  version: 1.0.0
host: api.linkedin.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /companies/{id}/historical-follow-statistics:
    get:
      summary: Get Companies Historical Follow Statistics
      description: Get companies  historical follow statistics
      operationId: getCompaniesHistoricalFollowStatistics
      x-api-path-slug: companiesidhistoricalfollowstatistics-get
      parameters:
      - in: query
        name: format
        description: The message format
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Companies
      - ""
      - Historical
      - Follow
      - Statistics
  /companies/{id}/historical-status-update-statistics:
    get:
      summary: Get Companies Historical Status Update Statistics
      description: Get companies  historical status update statistics
      operationId: getCompaniesHistoricalStatusUpdateStatistics
      x-api-path-slug: companiesidhistoricalstatusupdatestatistics-get
      parameters:
      - in: query
        name: format
        description: The message format
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Companies
      - ""
      - Historical
      - Status
      - Update
      - Statistics
  /companies/{id}/company-statistics:
    get:
      summary: Get Companies Company Statistics
      description: Get companies  company statistics
      operationId: getCompaniesCompanyStatistics
      x-api-path-slug: companiesidcompanystatistics-get
      parameters:
      - in: query
        name: format
        description: The message format
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Companies
      - ""
      - Company
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