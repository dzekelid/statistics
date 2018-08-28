---
swagger: "2.0"
x-collection-name: Actility
x-complete: 0
info:
  title: ThingPark DX Core API LRC packet statistics retrieval
  description: Retrieves packets statistics between the LRC and the base station corresponding
    to the provided base station ref, if that base station is within authorized scopes.
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /core/v141/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /deviceFrameStatistics:
    get:
      summary: Frame statistics retrieval
      description: Retrieves frame statistics of the devices corresponding to the
        provided parameters, if those devices are within authorized scopes.
      operationId: retrieves-frame-statistics-of-the-devices-corresponding-to-the-provided-parameters-if-those-devices-
      x-api-path-slug: deviceframestatistics-get
      parameters:
      - in: query
        name: aggregationStep
        description: Number of hours (between 1 and 24) used for aggregating the frame
          statistics
      - in: query
        name: baseStationId
        description: Id of the base station which received the frame
      - in: query
        name: deviceEUIList
        description: List of device EUIs for which device statistics should be retrieved
      - in: query
        name: duration
        description: Period (number of days) for which frame statistics should be
          retrieved
      - in: query
        name: startDate
        description: Start date in ISO 8601 format of the period for which frame statistics
          should be retrieved
      responses:
        200:
          description: OK
      tags:
      - Frame
      - Statistics
      - Retrieval
  /deviceHealthStatistics:
    get:
      summary: Health statistics retrieval
      description: Retrieves health statistics for all devices within authorized scopes.
      operationId: retrieves-health-statistics-for-all-devices-within-authorized-scopes
      x-api-path-slug: devicehealthstatistics-get
      responses:
        200:
          description: OK
      tags:
      - Health
      - Statistics
      - Retrieval
  /baseStationFrameStatistics:
    get:
      summary: Frame statistics retrieval
      description: Retrieves frame statistics of the base stations corresponding to
        the provided parameters, if those base stations are within authorized scopes.
      operationId: retrieves-frame-statistics-of-the-base-stations-corresponding-to-the-provided-parameters-if-those-ba
      x-api-path-slug: basestationframestatistics-get
      parameters:
      - in: query
        name: aggregationStep
        description: Number of hours (between 1 and 24) used for aggregating the frame
          statistics
      - in: query
        name: baseStationId
        description: Id of the base station for which frame statistics should be retrieved
      - in: query
        name: duration
        description: Period (number of days) for which frame statistics should be
          retrieved
      - in: query
        name: startDate
        description: Start date in ISO 8601 format of the period for which frame statistics
          should be retrieved
      responses:
        200:
          description: OK
      tags:
      - Frame
      - Statistics
      - Retrieval
  /baseStationHealthStatistics:
    get:
      summary: Health statistics retrieval
      description: Retrieves health statistics for all base stations within authorized
        scopes.
      operationId: retrieves-health-statistics-for-all-base-stations-within-authorized-scopes
      x-api-path-slug: basestationhealthstatistics-get
      responses:
        200:
          description: OK
      tags:
      - Health
      - Statistics
      - Retrieval
  /baseStations/{baseStationRef}/channels/{channelName}/signalStatistics:
    get:
      summary: Signal statistics retrieval
      description: Retrieves signal statistics (RSSI and SNR metrics) for a specific
        channel of the base station corresponding to the provided base station ref,
        if that base station is within authorized scopes.
      operationId: retrieves-signal-statistics-rssi-and-snr-metrics-for-a-specific-channel-of-the-base-station-correspo
      x-api-path-slug: basestationsbasestationrefchannelschannelnamesignalstatistics-get
      parameters:
      - in: path
        name: baseStationRef
        description: Ref of the base station for which signal statistics should be
          retrieved
      - in: path
        name: channelName
        description: Name of the channel for which signal statistics should be retrieved
      - in: query
        name: duration
        description: Period (number of hours) for which signal statistics should be
          retrieved
      - in: query
        name: startDate
        description: Start date in ISO 8601 format of the period for which signal
          statistics should be retrieved
      responses:
        200:
          description: OK
      tags:
      - Signal
      - Statistics
      - Retrieval
  /baseStations/{baseStationRef}/channels/{channelName}/dutyCycleStatistics:
    get:
      summary: Duty cycle statistics retrieval
      description: Retrieves duty cycle statistics for a specific channel of the base
        station corresponding to the provided base station ref, if that base station
        is within authorized scopes.
      operationId: retrieves-duty-cycle-statistics-for-a-specific-channel-of-the-base-station-corresponding-to-the-prov
      x-api-path-slug: basestationsbasestationrefchannelschannelnamedutycyclestatistics-get
      parameters:
      - in: query
        name: aggregationStep
        description: Number of hours (between 1 and 24) used for aggregating the duty
          cycle statistics
      - in: path
        name: baseStationRef
        description: Ref of the base station for which duty cycle statistics should
          be retrieved
      - in: path
        name: channelName
        description: Name of the channel for which duty cycle statistics should be
          retrieved
      - in: query
        name: duration
        description: Period (number of days between 1 and 7) for which duty cycle
          statistics should be retrieved
      - in: query
        name: startDate
        description: Start date in ISO 8601 format of the period for which duty cycle
          statistics should be retrieved
      responses:
        200:
          description: OK
      tags:
      - Duty
      - Cycle
      - Statistics
      - Retrieval
  /baseStations/{baseStationRef}/lrcPacketStatistics:
    get:
      summary: LRC packet statistics retrieval
      description: Retrieves packets statistics between the LRC and the base station
        corresponding to the provided base station ref, if that base station is within
        authorized scopes.
      operationId: retrieves-packets-statistics-between-the-lrc-and-the-base-station-corresponding-to-the-provided-base
      x-api-path-slug: basestationsbasestationreflrcpacketstatistics-get
      parameters:
      - in: query
        name: aggregationStep
        description: Number of hours (between 1 and 24) used for aggregating the LRC
          packet statistics
      - in: path
        name: baseStationRef
        description: Ref of the base station for which LRC packet statistics should
          be retrieved
      - in: query
        name: duration
        description: Period (number of days) for which LRC packet statistics should
          be retrieved
      - in: query
        name: startDate
        description: Start date in ISO 8601 format of the period for which LRC packet
          statistics should be retrieved
      responses:
        200:
          description: OK
      tags:
      - LRC
      - Packet
      - Statistics
      - Retrieval
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