swagger: "2.0"
x-collection-name: Xibo
x-complete: 1
info:
  title: Xibo API
  description: xibo-cms-api
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /displaygroup/{displayGroupId}/action/clearStatsAndLogs:
    post:
      summary: 'Action: Clear Stats and Logs'
      description: Clear all stats and logs on this Group
      operationId: displayGroupActionClearStatsAndLogs
      x-api-path-slug: displaygroupdisplaygroupidactionclearstatsandlogs-post
      parameters:
      - in: path
        name: displayGroupId
        description: The display group id
      responses:
        200:
          description: OK
      tags:
      - 'Action:'
      - Clear
      - Stats
      - Logs