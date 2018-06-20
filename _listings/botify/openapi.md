---
swagger: "2.0"
x-collection-name: Botify
x-complete: 1
info:
  title: Botify
  description: botify-saas-api
  version: 1.0.0
host: api.botify.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /analyses/{username}/{project_slug}/{analysis_slug}/crawl_statistics:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Crawl Statistics
      description: Get analyses username project slug analysis slug crawl statistics.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugCrawlStatistics
      x-api-path-slug: analysesusernameproject-sluganalysis-slugcrawl-statistics-get
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Crawl
      - Statistics
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Crawl Statistics
      description: Parameters analyses username project slug analysis slug crawl statistics.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugCrawlStatistics
      x-api-path-slug: analysesusernameproject-sluganalysis-slugcrawl-statistics-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Crawl
      - Statistics
  /analyses/{username}/{project_slug}/{analysis_slug}/crawl_statistics/time:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Crawl Statistics Time
      description: Return crawl statistics grouped by time frequency (1 min, 5 mins
        or 60 min) for an analysis
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugCrawlStatisticsTime
      x-api-path-slug: analysesusernameproject-sluganalysis-slugcrawl-statisticstime-get
      parameters:
      - in: query
        name: frequency
        description: Aggregation frequency
      - in: query
        name: limit
        description: max number of elements to retrieve
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Crawl
      - Statistics
      - Time
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Crawl Statistics
        Time
      description: Parameters analyses username project slug analysis slug crawl statistics
        time.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugCrawlStatisticsTime
      x-api-path-slug: analysesusernameproject-sluganalysis-slugcrawl-statisticstime-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Crawl
      - Statistics
      - Time
  /analyses/{username}/{project_slug}/{analysis_slug}/crawl_statistics/urls/{list_type}:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Crawl Statistics Urls
        List Type
      description: Return a list of 1000 latest URLs crawled (all crawled URLs or
        only URLS with HTTP errors)
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugCrawlStatisticsUrlsListType
      x-api-path-slug: analysesusernameproject-sluganalysis-slugcrawl-statisticsurlslist-type-get
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Crawl
      - Statistics
      - Urls
      - List
      - Type
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Crawl Statistics
        Urls List Type
      description: Parameters analyses username project slug analysis slug crawl statistics
        urls list type.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugCrawlStatisticsUrlsListType
      x-api-path-slug: analysesusernameproject-sluganalysis-slugcrawl-statisticsurlslist-type-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Crawl
      - Statistics
      - Urls
      - List
      - Type
---