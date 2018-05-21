---
swagger: "2.0"
x-collection-name: Auth0
x-complete: 1
info:
  title: Auth0 API
  description: auth0-exposes-two-apis-for-developers-to-consume-in-their-applications
  version: 1.0.0
host: login.auth0.com
basePath: api/v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /stats/active-users:
    get:
      summary: Get Stats Active Users
      description: Get stats active users.
      operationId: getStatsActiveUsers
      x-api-path-slug: statsactiveusers-get
      responses:
        200:
          description: OK
      tags:
      - Statistics
  /stats/daily:
    get:
      summary: Get Stats Daily
      description: Get stats daily.
      operationId: getStatsDaily
      x-api-path-slug: statsdaily-get
      parameters:
      - in: query
        name: from
        description: The first day of the period (inclusive) in YYYYMMDD format
      - in: query
        name: to
        description: The last day of the period (inclusive) in YYYYMMDD format
      responses:
        200:
          description: OK
      tags:
      - Statistics
      - Daily
---