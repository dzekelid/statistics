---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Get Stats
  description: |-
    **This endpoint allows you to retrieve all of your global email statistics between a given date range.**

    Parent accounts will see aggregated stats for their account and all subuser accounts. Subuser accounts will only see their own stats.
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /browsers/stats:
    get:
      summary: Get Browsers Stats
      description: |-
        **This endpoint allows you to retrieve your email statistics segmented by browser type.**

        **We only store up to 7 days of email activity in our database.** By default, 500 items will be returned per request via the Advanced Stats API endpoints.

        Advanced Stats provide a more in-depth view of your email statistics and the actions taken by your recipients. You can segment these statistics by geographic location, device type, client type, browser, and mailbox provider. For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html).
      operationId: browsers.stats.get
      x-api-path-slug: browsersstats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How to group the stats
      - in: query
        name: browsers
        description: The browsers to get statistics for
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: limit
        description: The number of results to include on each page
      - in: query
        name: No Name
      - in: query
        name: offset
        description: The number of results to exclude
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Browsers
      - Stats
  /categories/stats:
    get:
      summary: Get Categories Stats
      description: |-
        **This endpoint allows you to retrieve all of your email statistics for each of your categories.**

        If you do not define any query parameters, this endpoint will return a sum for each category in groups of 10.

        Categories allow you to group your emails together according to broad topics that you define. For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/categories.html).
      operationId: categories.stats.get
      x-api-path-slug: categoriesstats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How to group the statistics
      - in: query
        name: categories
        description: The individual categories that you want to retrieve statistics
          for
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: limit
        description: The number of results to include
      - in: query
        name: No Name
      - in: query
        name: offset
        description: The number of results to skip
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Categories
      - Stats
  /categories/stats/sums:
    get:
      summary: Get Categories Stats Sums
      description: |-
        **This endpoint allows you to retrieve the total sum of each email statistic for every category over the given date range.**

        If you do not define any query parameters, this endpoint will return a sum for each category in groups of 10.

        Categories allow you to group your emails together according to broad topics that you define. For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/categories.html).
      operationId: categories.stats.sums.get
      x-api-path-slug: categoriesstatssums-get
      parameters:
      - in: query
        name: aggregated_by
        description: How to group the statistics
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: limit
        description: Limits the number of results returned
      - in: query
        name: No Name
      - in: query
        name: offset
        description: The point in the list to begin retrieving results
      - in: query
        name: sort_by_direction
        description: The direction you want to sort
      - in: query
        name: sort_by_metric
        description: The metric that you want to sort by
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Categories
      - Stats
      - Sums
  /clients/stats:
    get:
      summary: Get Clients Stats
      description: |-
        **This endpoint allows you to retrieve your email statistics segmented by client type.**

        **We only store up to 7 days of email activity in our database.** By default, 500 items will be returned per request via the Advanced Stats API endpoints.

        Advanced Stats provide a more in-depth view of your email statistics and the actions taken by your recipients. You can segment these statistics by geographic location, device type, client type, browser, and mailbox provider. For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html).
      operationId: clients.stats.get
      x-api-path-slug: clientsstats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How to group the statistics
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: No Name
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Clients
      - Stats
  /clients/{client_type}/stats:
    get:
      summary: Get Clients Client Type Stats
      description: |-
        **This endpoint allows you to retrieve your email statistics segmented by a specific client type.**

        **We only store up to 7 days of email activity in our database.** By default, 500 items will be returned per request via the Advanced Stats API endpoints.

        ## Available Client Types
        - phone
        - tablet
        - webmail
        - desktop

        Advanced Stats provide a more in-depth view of your email statistics and the actions taken by your recipients. You can segment these statistics by geographic location, device type, client type, browser, and mailbox provider. For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html).
      operationId: clients.client_type.stats.get
      x-api-path-slug: clientsclient-typestats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How to group the statistics
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: No Name
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Clients
      - Client
      - Type
      - Stats
  /devices/stats:
    get:
      summary: Get Devices Stats
      description: "**This endpoint allows you to retrieve your email statistics segmented
        by the device type.**\n\n**We only store up to 7 days of email activity in
        our database.** By default, 500 items will be returned per request via the
        Advanced Stats API endpoints.\n\n## Available Device Types\n| **Device** |
        **Description** | **Example** |\n|---|---|---|\n| Desktop | Email software
        on desktop computer. | I.E., Outlook, Sparrow, or Apple Mail. |\n| Webmail
        |\tA web-based email client. | I.E., Yahoo, Google, AOL, or Outlook.com. |\n|
        Phone | A smart phone. | iPhone, Android, Blackberry, etc.\n| Tablet | A tablet
        computer. | iPad, android based tablet, etc. |\n| Other | An unrecognized
        device. |\n\nAdvanced Stats provide a more in-depth view of your email statistics
        and the actions taken by your recipients. You can segment these statistics
        by geographic location, device type, client type, browser, and mailbox provider.
        For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html)."
      operationId: devices.stats.get
      x-api-path-slug: devicesstats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How to group the statistics
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: limit
        description: How many results to include on each page
      - in: query
        name: No Name
      - in: query
        name: offset
        description: How many results to exclude
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Devices
      - Stats
  /geo/stats:
    get:
      summary: Get Geo Stats
      description: |-
        **This endpoint allows you to retrieve your email statistics segmented by country and state/province.**

        **We only store up to 7 days of email activity in our database.** By default, 500 items will be returned per request via the Advanced Stats API endpoints.

        Advanced Stats provide a more in-depth view of your email statistics and the actions taken by your recipients. You can segment these statistics by geographic location, device type, client type, browser, and mailbox provider. For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html).
      operationId: geo.stats.get
      x-api-path-slug: geostats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How you would like the statistics to be grouped
      - in: query
        name: country
        description: The country you would like to see statistics for
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: limit
        description: How many results to include on each page
      - in: query
        name: No Name
      - in: query
        name: offset
        description: How many results to exclude
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Geo
      - Stats
  /mailbox_providers/stats:
    get:
      summary: Get Mailbox Provers Stats
      description: |-
        **This endpoint allows you to retrieve your email statistics segmented by recipient mailbox provider.**

        **We only store up to 7 days of email activity in our database.** By default, 500 items will be returned per request via the Advanced Stats API endpoints.

        Advanced Stats provide a more in-depth view of your email statistics and the actions taken by your recipients. You can segment these statistics by geographic location, device type, client type, browser, and mailbox provider. For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html).
      operationId: mailbox_providers.stats.get
      x-api-path-slug: mailbox-providersstats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How to group the stats
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: limit
        description: The number of results to include on each page
      - in: query
        name: mailbox_providers
        description: The mail box providers to get statistics for
      - in: query
        name: No Name
      - in: query
        name: offset
        description: The number of results to exclude
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Mailbox
      - Provers
      - Stats
  /stats:
    get:
      summary: Get Stats
      description: |-
        **This endpoint allows you to retrieve all of your global email statistics between a given date range.**

        Parent accounts will see aggregated stats for their account and all subuser accounts. Subuser accounts will only see their own stats.
      operationId: GET_stats
      x-api-path-slug: stats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How to group the statistics
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: limit
        description: The number of results to return
      - in: query
        name: No Name
      - in: query
        name: offset
        description: The point in the list to begin retrieving results
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Stats
  /subusers/stats:
    get:
      summary: Get Subusers Stats
      description: |-
        **This endpoint allows you to retrieve the email statistics for the given subusers.**

        You may retrieve statistics for up to 10 different subusers by including an additional _subusers_ parameter for each additional subuser.

        While you can always view the statistics for all email activity on your account, subuser statistics enable you to view specific segments of your stats. Emails sent, bounces, and spam reports are always tracked for subusers. Unsubscribes, clicks, and opens are tracked if you have enabled the required settings.

        For more information, see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/subuser.html).
      operationId: subusers.stats.get
      x-api-path-slug: subusersstats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How to group the statistics
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: limit
        description: Limits the number of results returned per page
      - in: query
        name: offset
        description: The point in the list to begin retrieving results from
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      - in: query
        name: subusers
        description: The subuser you want to retrieve statistics for
      responses:
        200:
          description: OK
      tags:
      - Email
      - Subusers
      - Stats
  /subusers/stats/monthly:
    get:
      summary: Get Subusers Stats Monthly
      description: |-
        **This endpoint allows you to retrieve the monthly email statistics for all subusers over the given date range.**

        While you can always view the statistics for all email activity on your account, subuser statistics enable you to view specific segments of your stats for your subusers. Emails sent, bounces, and spam reports are always tracked for subusers. Unsubscribes, clicks, and opens are tracked if you have enabled the required settings.

        When using the `sort_by_metric` to sort your stats by a specific metric, you can not sort by the following metrics:
        `bounce_drops`, `deferred`, `invalid_emails`, `processed`, `spam_report_drops`, `spam_reports`, or `unsubscribe_drops`.

        For more information, see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/subuser.html).
      operationId: subusers.stats.monthly.get
      x-api-path-slug: subusersstatsmonthly-get
      parameters:
      - in: query
        name: date
        description: The date of the month to retrieve statistics for
      - in: query
        name: limit
        description: Optional field to limit the number of results returned
      - in: query
        name: offset
        description: Optional beginning point in the list to retrieve from
      - in: query
        name: sort_by_direction
        description: The direction you want to sort
      - in: query
        name: sort_by_metric
        description: The metric that you want to sort by
      - in: query
        name: subuser
        description: A substring search of your subusers
      responses:
        200:
          description: OK
      tags:
      - Email
      - Subusers
      - Stats
      - Monthly
  /subusers/stats/sums:
    get:
      summary: Get Subusers Stats Sums
      description: |-
        **This endpoint allows you to retrieve the total sums of each email statistic metric for all subusers over the given date range.**


        While you can always view the statistics for all email activity on your account, subuser statistics enable you to view specific segments of your stats. Emails sent, bounces, and spam reports are always tracked for subusers. Unsubscribes, clicks, and opens are tracked if you have enabled the required settings.

        For more information, see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/subuser.html).
      operationId: subusers.stats.sums.get
      x-api-path-slug: subusersstatssums-get
      parameters:
      - in: query
        name: aggregated_by
        description: How to group the statistics
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: limit
        description: Limits the number of results returned per page
      - in: query
        name: offset
        description: The point in the list to begin retrieving results from
      - in: query
        name: sort_by_direction
        description: The direction you want to sort
      - in: query
        name: sort_by_metric
        description: The metric that you want to sort by
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Subusers
      - Stats
      - Sums
  /subusers/{subuser_name}/stats/monthly:
    get:
      summary: Get Subusers Subuser Name Stats Monthly
      description: |-
        **This endpoint allows you to retrive the monthly email statistics for a specific subuser.**

        While you can always view the statistics for all email activity on your account, subuser statistics enable you to view specific segments of your stats for your subusers. Emails sent, bounces, and spam reports are always tracked for subusers. Unsubscribes, clicks, and opens are tracked if you have enabled the required settings.

        When using the `sort_by_metric` to sort your stats by a specific metric, you can not sort by the following metrics:
        `bounce_drops`, `deferred`, `invalid_emails`, `processed`, `spam_report_drops`, `spam_reports`, or `unsubscribe_drops`.

        For more information, see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/subuser.html).
      operationId: subusers.subuser_name.stats.monthly.get
      x-api-path-slug: subuserssubuser-namestatsmonthly-get
      parameters:
      - in: query
        name: date
        description: The date of the month to retrieve statistics for
      - in: query
        name: limit
        description: Optional field to limit the number of results returned
      - in: query
        name: offset
        description: Optional beginning point in the list to retrieve from
      - in: query
        name: sort_by_direction
        description: The direction you want to sort
      - in: query
        name: sort_by_metric
        description: The metric that you want to sort by
      responses:
        200:
          description: OK
      tags:
      - Email
      - Subusers
      - Subuser
      - Name
      - Stats
      - Monthly
  /user/webhooks/parse/stats:
    get:
      summary: Get User Webhooks Parse Stats
      description: |-
        **This endpoint allows you to retrieve the statistics for your Parse Webhook useage.**

        SendGrid's Inbound Parse Webhook allows you to parse the contents and attachments of incomming emails. The Parse API can then POST the parsed emails to a URL that you specify. The Inbound Parse Webhook cannot parse messages greater than 20MB in size, including all attachments.

        There are a number of pre-made integrations for the SendGrid Parse Webhook which make processing events easy. You can find these integrations in the [Library Index](https://sendgrid.com/docs/Integrate/libraries.html#-Webhook-Libraries).
      operationId: user.webhooks.parse.stats.get
      x-api-path-slug: userwebhooksparsestats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How you would like the statistics to by grouped
      - in: query
        name: end_date
        description: The end date of the statistics you want to retrieve
      - in: query
        name: limit
        description: The number of statistics to return on each page
      - in: query
        name: No Name
      - in: query
        name: offset
        description: The number of statistics to skip
      - in: query
        name: start_date
        description: The starting date of the statistics you want to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - User
      - Webhooks
      - Parse
      - Stats
  /alerts:
    get:
      summary: Get Alerts
      description: "**This endpoint allows you to retieve all of your alerts.**\n\nAlerts
        allow you to specify an email address to receive notifications regarding your
        email usage or statistics. \n* Usage alerts allow you to set the threshold
        at which an alert will be sent.\n* Stats notifications allow you to set how
        frequently you would like to receive email statistics reports. For example,
        \"daily\", \"weekly\", or \"monthly\".\n\nFor more information about alerts,
        please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/alerts.html)."
      operationId: GET_alerts
      x-api-path-slug: alerts-get
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Alerts
  /alerts/{alert_id}:
    delete:
      summary: Delete Alerts Alert
      description: "**This endpoint allows you to delete an alert.**\n\nAlerts allow
        you to specify an email address to receive notifications regarding your email
        usage or statistics. \n* Usage alerts allow you to set the threshold at which
        an alert will be sent.\n* Stats notifications allow you to set how frequently
        you would like to receive email statistics reports. For example, \"daily\",
        \"weekly\", or \"monthly\".\n\nFor more information about alerts, please see
        our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/alerts.html)."
      operationId: alerts.alert_id.delete
      x-api-path-slug: alertsalert-id-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Alerts
      - Alert
    get:
      summary: Get Alerts Alert
      description: "**This endpoint allows you to retrieve a specific alert.**\n\nAlerts
        allow you to specify an email address to receive notifications regarding your
        email usage or statistics. \n* Usage alerts allow you to set the threshold
        at which an alert will be sent.\n* Stats notifications allow you to set how
        frequently you would like to receive email statistics reports. For example,
        \"daily\", \"weekly\", or \"monthly\".\n\nFor more information about alerts,
        please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/alerts.html)."
      operationId: alerts.alert_id.get
      x-api-path-slug: alertsalert-id-get
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Alerts
      - Alert
    patch:
      summary: Patch Alerts Alert
      description: "**This endpoint allows you to update an alert.**\n\nAlerts allow
        you to specify an email address to receive notifications regarding your email
        usage or statistics. \n* Usage alerts allow you to set the threshold at which
        an alert will be sent.\n* Stats notifications allow you to set how frequently
        you would like to receive email statistics reports. For example, \"daily\",
        \"weekly\", or \"monthly\".\n\nFor more information about alerts, please see
        our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/alerts.html)."
      operationId: alerts.alert_id.patch
      x-api-path-slug: alertsalert-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Alerts
      - Alert
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---