swagger: "2.0"
x-collection-name: Mailgun
x-complete: 1
info:
  title: Mailgun API
  description: powerful-apis-that-allow-you-to-send-receive-and-track-email-effortlessly-
  version: v2
host: api.mailgun.net
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  stats/:
    get:
      summary: Stats
      description: Returns a list of event stat items. Each record represents counts
        for one event per one day.
      operationId: getStats
      x-api-path-slug: stats-get
      parameters:
      - in: query
        name: event
        description: Name of the event to receive the stats for
      - in: query
        name: limit
        description: Maximum number of records to return
      - in: query
        name: skip
        description: Number of records to skip
      - in: query
        name: start-date
        description: The date to receive the stats starting from
      responses:
        200:
          description: OK
      tags:
      - Stats