swagger: "2.0"
x-collection-name: APImetrics
x-complete: 1
info:
  title: APImetrics Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /calls/{id}/stats/before:
    get:
      summary: List Stats from before a date for an API Call
      description: List Stats from before a date for an API Call
      operationId: listStatsFromBeforeDateAPICall
      x-api-path-slug: callsidstatsbefore-get
      parameters:
      - in: path
        name: id
        description: ID string of API Call
      - in: query
        name: kind
        description: Granularity of data required, one of DAY, WEEK, MONTH, YEAR
      - in: query
        name: limit
        description: Maximum number of results to return
      - in: query
        name: location_id
        description: Location where the API Call was made
      - in: query
        name: time
        description: ISO formatted date string for the end of the period you wish
          to view
      - in: query
        name: type
        description: Return stats for all calls in the time period specified which
          had this result
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Calls
      - ""
      - Stats
      - Before
  /calls/{id}/stats/since:
    get:
      summary: List Stats since a date for an API Call
      description: List Stats since a date for an API Call
      operationId: listStatsSinceDateAPICall
      x-api-path-slug: callsidstatssince-get
      parameters:
      - in: path
        name: id
        description: ID string of API Call
      - in: query
        name: kind
        description: Granularity of data required, one of DAY, WEEK, MONTH, YEAR
      - in: query
        name: limit
        description: Maximum number of results to return
      - in: query
        name: location_id
        description: Location where the API Call was made
      - in: query
        name: time
        description: ISO formatted date string for the start of the period you wish
          to view
      - in: query
        name: type
        description: Return stats for all calls in the time period specified which
          had this result
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Calls
      - ""
      - Stats
      - Since