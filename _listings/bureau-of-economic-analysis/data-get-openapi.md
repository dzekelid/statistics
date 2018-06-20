---
swagger: "2.0"
x-collection-name: Bureau of Economic Analysis
x-complete: 0
info:
  title: The Bureau of Economic Analysis (BEA) API Economic Statistics
  description: Economic Statistics
  version: v1
host: www.bea.gov/api/data?&UserID=Your-36CharacterKey&method=getparameterlist&datasetname=RegionalData&
basePath: /api/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  data/:
    get:
      summary: Economic Statistics
      description: Economic Statistics
      operationId: getData
      x-api-path-slug: data-get
      parameters:
      - in: query
        name: datasetname
      - in: query
        name: method
      - in: query
        name: ParameterName
      - in: query
        name: ResultFormat
      - in: query
        name: UserID
        description: Your user id
      responses:
        200:
          description: OK
      tags:
      - Economic
      - Statistics
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