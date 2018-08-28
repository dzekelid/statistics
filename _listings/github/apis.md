---
name: GitHub
x-slug: github
description: GitHub brings together the worlds largest community of developers to
  discover, share, and build better software. From open source projects to private
  team repositories, were your all-in-one platform for collaborative development.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
x-kinRank: "10"
x-alexaRank: "64"
tags: Statistics
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/statistics/master/_listings/github/apis.md
specificationVersion: "0.14"
apis:
- name: GitHub - Get Repos Owner Repo Stats Code Frequency
  x-api-slug: reposownerrepostatscode-frequency-get
  description: |-
    Get the number of additions and deletions per week.
    Returns a weekly aggregate of the number of additions and deletions pushed
    to a repository.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statistics/master/_listings/github/reposownerrepostatscode-frequency-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statistics/master/_listings/github/reposownerrepostatscode-frequency-get-openapi.md
- name: GitHub - Get Repos Owner Repo Stats Commit Activity
  x-api-slug: reposownerrepostatscommit-activity-get
  description: |-
    Get the last year of commit activity data.
    Returns the last year of commit activity grouped by week. The days array
    is a group of commits per day, starting on Sunday.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statistics/master/_listings/github/reposownerrepostatscommit-activity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statistics/master/_listings/github/reposownerrepostatscommit-activity-get-openapi.md
- name: GitHub - Get Repos Owner Repo Stats Contributors
  x-api-slug: reposownerrepostatscontributors-get
  description: Get contributors list with additions, deletions, and commit counts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statistics/master/_listings/github/reposownerrepostatscontributors-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statistics/master/_listings/github/reposownerrepostatscontributors-get-openapi.md
- name: GitHub - Get Repos Owner Repo Stats Participation
  x-api-slug: reposownerrepostatsparticipation-get
  description: Get the weekly commit count for the repo owner and everyone else.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statistics/master/_listings/github/reposownerrepostatsparticipation-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statistics/master/_listings/github/reposownerrepostatsparticipation-get-openapi.md
- name: GitHub - Get Repos Owner Repo Stats Punch Card
  x-api-slug: reposownerrepostatspunch-card-get
  description: |-
    Get the number of commits per hour in each day.
    Each array contains the day number, hour number, and number of commits
    0-6 Sunday - Saturday
    0-23 Hour of day
    Number of commits

    For example, [2, 14, 25] indicates that there were 25 total commits, during
    the 2.00pm hour on Tuesdays. All times are based on the time zone of
    individual commits.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statistics/master/_listings/github/reposownerrepostatspunch-card-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statistics/master/_listings/github/reposownerrepostatspunch-card-get-openapi.md
- name: GitHub - Get Repos Owner Repo Stats Punch Card
  x-api-slug: reposownerrepostatspunch-card-get
  description: |-
    Get the number of commits per hour in each day.
    Each array contains the day number, hour number, and number of commits
    0-6 Sunday - Saturday
    0-23 Hour of day
    Number of commits

    For example, [2, 14, 25] indicates that there were 25 total commits, during
    the 2.00pm hour on Tuesdays. All times are based on the time zone of
    individual commits.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statistics/master/_listings/github/reposownerrepostatspunch-card-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statistics/master/_listings/github/reposownerrepostatspunch-card-get-openapi.md
- name: GitHub - Get Repos Owner Repo Stats Participation
  x-api-slug: reposownerrepostatsparticipation-get
  description: Get the weekly commit count for the repo owner and everyone else.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statistics/master/_listings/github/reposownerrepostatsparticipation-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statistics/master/_listings/github/reposownerrepostatsparticipation-get-openapi.md
- name: GitHub - Get Repos Owner Repo Stats Contributors
  x-api-slug: reposownerrepostatscontributors-get
  description: Get contributors list with additions, deletions, and commit counts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statistics/master/_listings/github/reposownerrepostatscontributors-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statistics/master/_listings/github/reposownerrepostatscontributors-get-openapi.md
- name: GitHub - Get Repos Owner Repo Stats Commit Activity
  x-api-slug: reposownerrepostatscommit-activity-get
  description: |-
    Get the last year of commit activity data.
    Returns the last year of commit activity grouped by week. The days array
    is a group of commits per day, starting on Sunday.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statistics/master/_listings/github/reposownerrepostatscommit-activity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statistics/master/_listings/github/reposownerrepostatscommit-activity-get-openapi.md
- name: GitHub - Get Repos Owner Repo Stats Code Frequency
  x-api-slug: reposownerrepostatscode-frequency-get
  description: |-
    Get the number of additions and deletions per week.
    Returns a weekly aggregate of the number of additions and deletions pushed
    to a repository.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statistics/master/_listings/github/reposownerrepostatscode-frequency-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statistics/master/_listings/github/reposownerrepostatscode-frequency-get-openapi.md
x-common:
- type: x--net-library
  url: https://github.com/octokit/octokit.net
- type: x-api-gallery
  url: http://giphy.api.gallery.streamdata.io
- type: x-api-stack
  url: http://github.stack.network
- type: x-base
  url: https://api.github.com
- type: x-blog
  url: http://github.com/blog
- type: x-blog-rss
  url: https://github.com/blog/subscribe
- type: x-change-log
  url: https://developer.github.com/changes/
- type: x-contact-form
  url: https://github.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/github
- type: x-crunchbase
  url: https://crunchbase.com/organization/github
- type: x-developer
  url: https://developer.github.com/
- type: x-github
  url: https://github.com/github
- type: x-guides
  url: https://developer.github.com/guides/
- type: x-ios-sdk
  url: https://github.com/octokit/octokit.objc
- type: x-pricing
  url: https://github.com/pricing
- type: x-privacy
  url: http://help.github.com/privacy-policy/
- type: x-ruby-library
  url: https://github.com/octokit/octokit.rb
- type: x-security
  url: http://help.github.com/security/
- type: x-status
  url: https://status.github.com/
- type: x-terms-of-service
  url: http://help.github.com/terms-of-service/
- type: x-transparency-report
  url: https://github.com/blog/1987-github-s-2014-transparency-report
- type: x-twitter
  url: https://twitter.com/github
- type: x-webhooks
  url: https://developer.github.com/webhooks/
- type: x-website
  url: https://github.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---