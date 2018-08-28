swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/admin/statistics:
    get:
      summary: Get Admin Statistics
      description: Get admin statistics.
      operationId: getApiV1AdminStatistics
      x-api-path-slug: apiv1adminstatistics-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Statistics
  /api/v1/admin/statistics/{type}:
    get:
      summary: Get Admin Statistics Type
      description: Get admin statistics type.
      operationId: getApiV1AdminStatisticsType
      x-api-path-slug: apiv1adminstatisticstype-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: type
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Statistics
      - Type
  /api/v1/admin/event/statistic:
    get:
      summary: Get Admin Event Statistic
      description: Get admin event statistic.
      operationId: getApiV1AdminEventStatistic
      x-api-path-slug: apiv1admineventstatistic-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Statistic
  /api/v1/admin/moderator/statistic:
    get:
      summary: Get Admin Moderator Statistic
      description: Get admin moderator statistic.
      operationId: getApiV1AdminModeratorStatistic
      x-api-path-slug: apiv1adminmoderatorstatistic-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Moderator
      - Statistic
  /api/v1/admin/parser/statistic:
    get:
      summary: Get Admin Parser Statistic
      description: Get admin parser statistic.
      operationId: getApiV1AdminParserStatistic
      x-api-path-slug: apiv1adminparserstatistic-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Parser
      - Statistic
  /api/v1/admin/place/statistic:
    get:
      summary: Get Admin Place Statistic
      description: Get admin place statistic.
      operationId: getApiV1AdminPlaceStatistic
      x-api-path-slug: apiv1adminplacestatistic-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Place
      - Statistic