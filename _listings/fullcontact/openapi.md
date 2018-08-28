swagger: "2.0"
x-collection-name: FullContact
x-complete: 1
info:
  title: FullContact Location API
  description: the-api-for-managing-fullcontact-locations
  termsOfService: https://www.fullcontact.com/terms/
  version: 1.0.0
host: api.fullcontact.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /stats.json:
    get:
      summary: Get Account Stats
      description: Get Account Stats
      operationId: getAccountStats
      x-api-path-slug: stats-json-get
      parameters:
      - in: query
        name: apiKey
        description: This API key is assigned to you by FullContact
      - in: query
        name: period
        description: You can define the month that you want to see usage stats for
          by using the period parameter
      responses:
        200:
          description: OK
      tags:
      - Statistics