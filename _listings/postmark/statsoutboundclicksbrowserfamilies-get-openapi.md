---
swagger: "2.0"
x-collection-name: Postmark
x-complete: 0
info:
  title: Postmark Get Stats Outbound Clicks Browserfamilies
  description: Get stats outbound clicks browserfamilies.
  version: 1.0.0
host: spamcheck.postmarkapp.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /stats/outbound:
    get:
      summary: Get Stats Outbound
      description: Get stats outbound.
      operationId: getStatsOutbound
      x-api-path-slug: statsoutbound-get
      parameters:
      - in: query
        name: fromdate
        description: Filter stats starting from the date specified
      - in: query
        name: tag
        description: Filter by tag
      - in: query
        name: todate
        description: Filter stats up to the date specified
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Stats
      - Outbound
  /stats/outbound/bounces:
    get:
      summary: Get Stats Outbound Bounces
      description: Get stats outbound bounces.
      operationId: getStatsOutboundBounces
      x-api-path-slug: statsoutboundbounces-get
      parameters:
      - in: query
        name: fromdate
        description: Filter stats starting from the date specified
      - in: query
        name: tag
        description: Filter by tag
      - in: query
        name: todate
        description: Filter stats up to the date specified
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Stats
      - Outbound
      - Bounces
  /stats/outbound/clicks:
    get:
      summary: Get Stats Outbound Clicks
      description: Get stats outbound clicks.
      operationId: getStatsOutboundClicks
      x-api-path-slug: statsoutboundclicks-get
      parameters:
      - in: query
        name: fromdate
        description: Filter stats starting from the date specified
      - in: query
        name: tag
        description: Filter by tag
      - in: query
        name: todate
        description: Filter stats up to the date specified
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Stats
      - Outbound
      - Clicks
  /stats/outbound/clicks/browserfamilies:
    get:
      summary: Get Stats Outbound Clicks Browserfamilies
      description: Get stats outbound clicks browserfamilies.
      operationId: getStatsOutboundClicksBrowserfamilies
      x-api-path-slug: statsoutboundclicksbrowserfamilies-get
      parameters:
      - in: query
        name: fromdate
        description: Filter stats starting from the date specified
      - in: query
        name: tag
        description: Filter by tag
      - in: query
        name: todate
        description: Filter stats up to the date specified
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Stats
      - Outbound
      - Clicks
      - Browserfamilies
  /stats/outbound/clicks/location:
    get:
      summary: Get Stats Outbound Clicks Location
      description: Get stats outbound clicks location.
      operationId: getStatsOutboundClicksLocation
      x-api-path-slug: statsoutboundclickslocation-get
      parameters:
      - in: query
        name: fromdate
        description: Filter stats starting from the date specified
      - in: query
        name: tag
        description: Filter by tag
      - in: query
        name: todate
        description: Filter stats up to the date specified
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Stats
      - Outbound
      - Clicks
      - Location
  /stats/outbound/clicks/platforms:
    get:
      summary: Get Stats Outbound Clicks Platforms
      description: Get stats outbound clicks platforms.
      operationId: getStatsOutboundClicksPlatforms
      x-api-path-slug: statsoutboundclicksplatforms-get
      parameters:
      - in: query
        name: fromdate
        description: Filter stats starting from the date specified
      - in: query
        name: tag
        description: Filter by tag
      - in: query
        name: todate
        description: Filter stats up to the date specified
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Stats
      - Outbound
      - Clicks
      - Platforms
  /stats/outbound/opens:
    get:
      summary: Get Stats Outbound Opens
      description: Get stats outbound opens.
      operationId: getStatsOutboundOpens
      x-api-path-slug: statsoutboundopens-get
      parameters:
      - in: query
        name: fromdate
        description: Filter stats starting from the date specified
      - in: query
        name: tag
        description: Filter by tag
      - in: query
        name: todate
        description: Filter stats up to the date specified
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Stats
      - Outbound
      - Opens
  /stats/outbound/opens/emailclients:
    get:
      summary: Get Stats Outbound Opens Emailclients
      description: Get stats outbound opens emailclients.
      operationId: getStatsOutboundOpensEmailclients
      x-api-path-slug: statsoutboundopensemailclients-get
      parameters:
      - in: query
        name: fromdate
        description: Filter stats starting from the date specified
      - in: query
        name: tag
        description: Filter by tag
      - in: query
        name: todate
        description: Filter stats up to the date specified
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Stats
      - Outbound
      - Opens
      - Emailclients
  /stats/outbound/opens/platforms:
    get:
      summary: Get Stats Outbound Opens Platforms
      description: Get stats outbound opens platforms.
      operationId: getStatsOutboundOpensPlatforms
      x-api-path-slug: statsoutboundopensplatforms-get
      parameters:
      - in: query
        name: fromdate
        description: Filter stats starting from the date specified
      - in: query
        name: tag
        description: Filter by tag
      - in: query
        name: todate
        description: Filter stats up to the date specified
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Stats
      - Outbound
      - Opens
      - Platforms
  /stats/outbound/opens/readtimes:
    get:
      summary: Get Stats Outbound Opens Readtimes
      description: Get stats outbound opens readtimes.
      operationId: getStatsOutboundOpensReadtimes
      x-api-path-slug: statsoutboundopensreadtimes-get
      parameters:
      - in: query
        name: fromdate
        description: Filter stats starting from the date specified
      - in: query
        name: tag
        description: Filter by tag
      - in: query
        name: todate
        description: Filter stats up to the date specified
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Stats
      - Outbound
      - Opens
      - Readtimes
  /stats/outbound/sends:
    get:
      summary: Get Stats Outbound Sends
      description: Get stats outbound sends.
      operationId: getStatsOutboundSends
      x-api-path-slug: statsoutboundsends-get
      parameters:
      - in: query
        name: fromdate
        description: Filter stats starting from the date specified
      - in: query
        name: tag
        description: Filter by tag
      - in: query
        name: todate
        description: Filter stats up to the date specified
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Stats
      - Outbound
      - Sends
  /stats/outbound/spam:
    get:
      summary: Get Stats Outbound Spam
      description: Get stats outbound spam.
      operationId: getStatsOutboundSpam
      x-api-path-slug: statsoutboundspam-get
      parameters:
      - in: query
        name: fromdate
        description: Filter stats starting from the date specified
      - in: query
        name: tag
        description: Filter by tag
      - in: query
        name: todate
        description: Filter stats up to the date specified
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Stats
      - Outbound
      - Spam
  /stats/outbound/tracked:
    get:
      summary: Get Stats Outbound Tracked
      description: Get stats outbound tracked.
      operationId: getStatsOutboundTracked
      x-api-path-slug: statsoutboundtracked-get
      parameters:
      - in: query
        name: fromdate
        description: Filter stats starting from the date specified
      - in: query
        name: tag
        description: Filter by tag
      - in: query
        name: todate
        description: Filter stats starting from the date specified
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Stats
      - Outbound
      - Tracked
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