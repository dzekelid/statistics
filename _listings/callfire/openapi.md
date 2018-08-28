swagger: "2.0"
x-collection-name: CallFire
x-complete: 1
info:
  title: CallFire
  description: callfire
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /calls/broadcasts/{id}/stats:
    get:
      summary: Get statistics on call broadcast
      description: Returns broadcast statistics like total number of sent/received
        actions, total cost, number of remaining outbound actions, error count, etc
      operationId: getCallBroadcastStats
      x-api-path-slug: callsbroadcastsidstats-get
      parameters:
      - in: query
        name: begin
        description: Start of the search time interval, formatted in unix time milliseconds
      - in: query
        name: end
        description: End of the search time interval, formatted in unix time milliseconds
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a call broadcast
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
      - Stats
  /texts/broadcasts/{id}/stats:
    get:
      summary: Get statistics on text broadcast
      description: 'Returns the broadcast statistics. Example: total number of the
        sent/received actions, total cost, number of remaining outbound actions, error
        count, etc'
      operationId: getTextBroadcastStats
      x-api-path-slug: textsbroadcastsidstats-get
      parameters:
      - in: query
        name: begin
        description: Start of a search find time interval, formatted in unix time
          milliseconds
      - in: query
        name: end
        description: End of a search time interval, formatted in unix time milliseconds
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a text broadcast
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Broadcasts
      - Stats