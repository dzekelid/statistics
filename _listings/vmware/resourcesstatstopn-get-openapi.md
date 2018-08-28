---
swagger: "2.0"
x-collection-name: VMWare
x-complete: 0
info:
  title: VMWare vRealize Operations Get TopN Stats
  description: 'TODO: Add Description'
  version: 1.0.0
host: example.com
basePath: /suite-api/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /resources/7a3a3bfc-1664-4e1d-bfe1-0e42db1d3c0e/stats:
    get:
      summary: Get Stats from Resource (Not query)
      description: I have not tested but you may be able to use the "resourceIds"
        input paramter to specify multiple resources (of the same kind, obviously).  The
        example here shows a daily avg for 30 days.  Timestamps are milli from epoch.
      operationId: Resources7a3a3bfc16644e1dBfe10e42db1d3c0eStatsGet
      x-api-path-slug: resources7a3a3bfc16644e1dbfe10e42db1d3c0estats-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: begin
      - in: query
        name: end
      - in: query
        name: intervalQuantifier
      - in: query
        name: intervalType
      - in: query
        name: rollUpType
      - in: query
        name: statKey
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Stats
  /resources/stats/topn:
    get:
      summary: Get TopN Stats
      description: 'TODO: Add Description'
      operationId: ResourcesStatsTopnGet
      x-api-path-slug: resourcesstatstopn-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: begin
      - in: header
        name: Content-Type
      - in: query
        name: intervalQuantifier
      - in: query
        name: intervalType
      - in: query
        name: rollUpType
      - in: query
        name: statKey
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Stats
      - Topn
  /api/resources/{resourceId}/stats:
    post:
      summary: Add or Update Stats of a Resource
      description: 'TODO: Add Description'
      operationId: ApiResourcesStatsByResourceIdPost
      x-api-path-slug: apiresourcesresourceidstats-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: resourceId
      responses:
        200:
          description: OK
      tags:
      - Resources
      - ResourceId
      - Stats
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