swagger: "2.0"
x-collection-name: GitHub
x-complete: 1
info:
  title: GitHub
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repos/{owner}/{repo}/stats/code_frequency:
    get:
      summary: Get Repos Owner Repo Stats Code Frequency
      description: |-
        Get the number of additions and deletions per week.
        Returns a weekly aggregate of the number of additions and deletions pushed
        to a repository.
      operationId: get-the-number-of-additions-and-deletions-per-weekreturns-a-weekly-aggregate-of-the-number-of-additi
      x-api-path-slug: reposownerrepostatscode-frequency-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Stats
      - Code
      - Frequency
      - Aggregation
  /repos/{owner}/{repo}/stats/commit_activity:
    get:
      summary: Get Repos Owner Repo Stats Commit Activity
      description: |-
        Get the last year of commit activity data.
        Returns the last year of commit activity grouped by week. The days array
        is a group of commits per day, starting on Sunday.
      operationId: get-the-last-year-of-commit-activity-datareturns-the-last-year-of-commit-activity-grouped-by-week-th
      x-api-path-slug: reposownerrepostatscommit-activity-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Stats
      - Commit
      - Activity
  /repos/{owner}/{repo}/stats/contributors:
    get:
      summary: Get Repos Owner Repo Stats Contributors
      description: Get contributors list with additions, deletions, and commit counts.
      operationId: get-contributors-list-with-additions-deletions-and-commit-counts
      x-api-path-slug: reposownerrepostatscontributors-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Stats
      - Contributors
  /repos/{owner}/{repo}/stats/participation:
    get:
      summary: Get Repos Owner Repo Stats Participation
      description: Get the weekly commit count for the repo owner and everyone else.
      operationId: get-the-weekly-commit-count-for-the-repo-owner-and-everyone-else
      x-api-path-slug: reposownerrepostatsparticipation-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Stats
      - Participation
  /repos/{owner}/{repo}/stats/punch_card:
    get:
      summary: Get Repos Owner Repo Stats Punch Card
      description: |-
        Get the number of commits per hour in each day.
        Each array contains the day number, hour number, and number of commits
        0-6 Sunday - Saturday
        0-23 Hour of day
        Number of commits

        For example, [2, 14, 25] indicates that there were 25 total commits, during
        the 2.00pm hour on Tuesdays. All times are based on the time zone of
        individual commits.
      operationId: get-the-number-of-commits-per-hour-in-each-dayeach-array-contains-the-day-number-hour-number-and-num
      x-api-path-slug: reposownerrepostatspunch-card-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Stats
      - Punch
      - Card