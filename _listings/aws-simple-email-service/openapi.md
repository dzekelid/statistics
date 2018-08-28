swagger: "2.0"
x-collection-name: AWS Simple Email Service
x-complete: 1
info:
  title: AWS Simple Email Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetSendStatistics:
    get:
      summary: Get Send Statistics
      description: Returns the user's sending statistics.
      operationId: getSendStatistics
      x-api-path-slug: actiongetsendstatistics-get
      parameters:
      - in: query
        name: SendDataPoints.member.N
        description: A list of data points, each of which represents 15 minutes of
          activity
        type: string
      responses:
        200:
          description: OK
      tags:
      - Send Statistics