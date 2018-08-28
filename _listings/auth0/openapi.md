swagger: "2.0"
x-collection-name: Auth0
x-complete: 1
info:
  title: Auth0 Users API
  version: v1
host: login.auth0.com
basePath: /users
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
  /api/v2/stats/active-users:
    get:
      summary: Get Active Users
      description: Gets the active users count (logged in during the last 30 days).
      operationId: get_active-users
      x-api-path-slug: apiv2statsactiveusers-get
      responses:
        200:
          description: OK
      tags:
      - Stats
      - Active
      - Users
  /api/v2/stats/daily:
    get:
      summary: Get Daily Stats
      description: Gets the daily stats for a particular period.
      operationId: get_daily
      x-api-path-slug: apiv2statsdaily-get
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
      - Stats
      - Daily