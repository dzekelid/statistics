---
swagger: "2.0"
x-collection-name: Azure Data Lake Analytics
x-complete: 0
info:
  title: Azure Data Lake Analytics API Job Get Statistics
  description: Gets statistics of the specified job.
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /catalog/usql/databases/{databaseName}/schemas/{schemaName}/tables/{tableName}/statistics:
    get:
      summary: Catalog List Table Statistics
      description: Retrieves the list of table statistics from the Data Lake Analytics
        catalog.
      operationId: Catalog_ListTableStatistics
      x-api-path-slug: catalogusqldatabasesdatabasenameschemasschemanametablestablenamestatistics-get
      parameters:
      - in: query
        name: $count
        description: The Boolean value of true or false to request a count of the
          matching resources included with the resources in the response, e
      - in: query
        name: $filter
        description: OData filter
      - in: query
        name: $orderby
        description: OrderBy clause
      - in: query
        name: $select
        description: OData Select statement
      - in: query
        name: $skip
        description: The number of items to skip over before returning elements
      - in: query
        name: $top
        description: The number of items to return
      - in: path
        name: databaseName
        description: The name of the database containing the statistics
      - in: query
        name: No Name
      - in: path
        name: schemaName
        description: The name of the schema containing the statistics
      - in: path
        name: tableName
        description: The name of the table containing the statistics
      responses:
        200:
          description: OK
      tags:
      - Catalog Table Statistics
  /Jobs/{jobIdentity}/GetStatistics:
    get:
      summary: Job Get Statistics
      description: Gets statistics of the specified job.
      operationId: Job_GetStatistics
      x-api-path-slug: jobsjobidentitygetstatistics-get
      parameters:
      - in: path
        name: jobIdentity
        description: Job Information ID
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Job Statistics
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