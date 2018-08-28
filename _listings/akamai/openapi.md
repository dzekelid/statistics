---
swagger: "2.0"
x-collection-name: Akamai
x-complete: 1
info:
  title: Akamai API
  description: the-akamai-api-for-managing-your-akamai-service
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /billing-center-api/v2/contracts/{contractId}/products/{productId}/statistics:
    get:
      summary: List Statistics per Contract
      description: List Statistics per Contract
      operationId: billingcenterapiv2contractscontractidproductsproductidstatisticsyearmonthfromyearfrommonthtoyeartomo
      x-api-path-slug: billingcenterapiv2contractscontractidproductsproductidstatistics-get
      parameters:
      - in: query
        name: contractId
        description: Identifies the contract under which data is aggregated
        type: string
      - in: query
        name: fromMonth
        description: The month starting the range of aggregated data
        type: string
      - in: query
        name: fromYear
        description: The year starting the range of aggregated data
        type: string
      - in: query
        name: month
        description: The month for which data is aggregated
        type: string
      - in: query
        name: productId
        description: Identifies the product under which data is aggregated
        type: string
      - in: query
        name: toMonth
        description: The month ending the range of aggregated data
        type: string
      - in: query
        name: toYear
        description: The year ending the range of aggregated data
        type: string
      - in: query
        name: year
        description: The year for which data is aggregated
        type: string
      responses:
        200:
          description: OK
      tags:
      - Billing
      - Center
      - Contracts
      - Contract
      - Products
      - Product
      - Statistics
      - Year
      - month
      - fromyear
      - frommonth
      - toyear
      - tomonth
  /billing-center-api/v2/reporting-groups/{reportingGroupId}/products/{productId}/statistics:
    get:
      summary: List Statistics per Reporting Group
      description: List Statistics per Reporting Group
      operationId: billingcenterapiv2reportinggroupsreportinggroupidproductsproductidstatisticsyearmonthfromyearfrommon
      x-api-path-slug: billingcenterapiv2reportinggroupsreportinggroupidproductsproductidstatistics-get
      parameters:
      - in: query
        name: fromMonth
        description: The month starting the range of aggregated data
        type: string
      - in: query
        name: fromYear
        description: The year starting the range of aggregated data
        type: string
      - in: query
        name: month
        description: The month for which data is aggregated
        type: string
      - in: query
        name: productId
        description: Identifies the product under which data is aggregated
        type: string
      - in: query
        name: reportingGroupId
        description: Identifies the unique reporting group
        type: string
      - in: query
        name: toMonth
        description: The month ending the range of aggregated data
        type: string
      - in: query
        name: toYear
        description: The year ending the range of aggregated data
        type: string
      - in: query
        name: year
        description: The year for which data is aggregated
        type: string
      responses:
        200:
          description: OK
      tags:
      - Billing
      - Center
      - Reporting
      - Groups
      - Reportinggroup
      - Products
      - Product
      - Statistics
      - Year
      - month
      - fromyear
      - frommonth
      - toyear
      - tomonth
---