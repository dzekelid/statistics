swagger: "2.0"
x-collection-name: Strava
x-complete: 1
info:
  title: Strava API v3
  description: strava-api
  version: 1.0.0
host: www.strava.com
basePath: /api/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /athletes/{id}/stats:
    get:
      summary: Get Athlete Stats
      description: Returns the activity stats of an athlete.
      operationId: getStats
      x-api-path-slug: athletesidstats-get
      parameters:
      - in: path
        name: id
        description: The identifier of the athlete
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - Athlete
      - Stats