swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost
  version: 1.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /channels/{channel_id}/stats:
    get:
      summary: Get channel statistics
      description: |-
        Get statistics for a channel.
        ##### Permissions
        Must have the `read_channel` permission.
      operationId: get-statistics-for-a-channel-permissionsmust-have-the-read-channel-permission
      x-api-path-slug: channelschannel-idstats-get
      parameters:
      - in: path
        name: channel_id
        description: Channel GUID
      responses:
        200:
          description: OK
      tags:
      - Channel
      - Statistics
  /teams/{team_id}/stats:
    get:
      summary: Get a team stats
      description: |-
        Get a team stats on the system.
        ##### Permissions
        Must be authenticated and have the `view_team` permission.
      operationId: get-a-team-stats-on-the-system-permissionsmust-be-authenticated-and-have-the-view-team-permission
      x-api-path-slug: teamsteam-idstats-get
      parameters:
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Team
      - Stats