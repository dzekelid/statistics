swagger: "2.0"
x-collection-name: AWS CloudWatch
x-complete: 1
info:
  title: AWS CloudWatch API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetMetricStatistics:
    "":
      summary: Get Metric Statistics
      description: Gets statistics for the specified metric.
      operationId: getmetricstatistics
      x-api-path-slug: actiongetmetricstatistics-
      parameters:
      - in: query
        name: Dimensions.member.N
        description: The dimensions
        type: string
      - in: query
        name: EndTime
        description: The time stamp that determines the last data point to return
        type: string
      - in: query
        name: ExtendedStatistics.member.N
        description: The percentile statistics
        type: string
      - in: query
        name: MetricName
        description: The name of the metric, with or without spaces
        type: string
      - in: query
        name: Namespace
        description: The namespace of the metric, with or without spaces
        type: string
      - in: query
        name: Period
        description: The granularity, in seconds, of the returned data points
        type: string
      - in: query
        name: StartTime
        description: The time stamp that determines the first data point to return
        type: string
      - in: query
        name: Statistics.member.N
        description: The metric statistics, other than percentile
        type: string
      - in: query
        name: Unit
        description: The unit for a given metric
        type: string
      responses:
        200:
          description: OK
      tags:
      - Metric Statistics