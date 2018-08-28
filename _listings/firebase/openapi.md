---
swagger: "2.0"
x-collection-name: Firebase
x-complete: 1
info:
  title: Firebase Dynamic Links
  description: programmatically-creates-and-manages-firebase-dynamic-links
  contact:
    name: Google
    url: https://google.com
  version: 1.0.0
host: firebasedynamiclinks-ipv6.googleapis.com
basePath: v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{dynamicLink}/linkStats:
    get:
      summary: Get Dynamiclink Linkstats
      description: |-
        Fetches analytics stats of a short Dynamic Link for a given
        duration. Metrics include number of clicks, redirects, installs,
        app first opens, and app reopens.
      operationId: firebasedynamiclinks.getLinkStats
      x-api-path-slug: dynamiclinklinkstats-get
      parameters:
      - in: query
        name: durationDays
        description: The span of time requested in days
      - in: path
        name: dynamicLink
        description: Dynamic Link URL
      responses:
        200:
          description: OK
      tags:
      - Dynammic
      - Links
      - Statistics
---