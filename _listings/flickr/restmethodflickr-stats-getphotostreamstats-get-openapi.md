---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Stats Get Photostream Stats
  description: Get the number of views on a user's photostream for a given date.
  version: 1.0.0
host: api.flickr.com
basePath: /services/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/?method=flickr.stats.getCollectionDomains:
    get:
      summary: Stats Get Collection Domains
      description: Get a list of referring domains for a collection
      operationId: getRestMethodFlickr.stats.getcollectiondomains
      x-api-path-slug: restmethodflickr-stats-getcollectiondomains-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: collection_id
        description: The id of the collection to get stats for
      - in: query
        name: date
        description: Stats will be returned for this date
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of domains to return per page
      responses:
        200:
          description: OK
      tags:
      - Stats
      - GetCollectionDomains
  /rest/?method=flickr.stats.getCollectionReferrers:
    get:
      summary: Stats Get Collection Referrers
      description: Get a list of referrers from a given domain to a collection
      operationId: getRestMethodFlickr.stats.getcollectionreferrers
      x-api-path-slug: restmethodflickr-stats-getcollectionreferrers-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: collection_id
        description: The id of the collection to get stats for
      - in: query
        name: date
        description: Stats will be returned for this date
      - in: query
        name: domain
        description: The domain to return referrers for
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of domains to return per page
      responses:
        200:
          description: OK
      tags:
      - Stats
      - GetCollectionReferrers
  /rest/?method=flickr.stats.getCollectionStats:
    get:
      summary: Stats Get Collection Stats
      description: Get the number of views on a collection for a given date.
      operationId: getRestMethodFlickr.stats.getcollectionstats
      x-api-path-slug: restmethodflickr-stats-getcollectionstats-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: collection_id
        description: The id of the collection to get stats for
      - in: query
        name: date
        description: Stats will be returned for this date
      - in: query
        name: format
        description: Response format
      responses:
        200:
          description: OK
      tags:
      - Stats
      - GetCollectionStats
  /rest/?method=flickr.stats.getPhotoDomains:
    get:
      summary: Stats Get Photo Domains
      description: Get a list of referring domains for a photo.
      operationId: getRestMethodFlickr.stats.getphotodomains
      x-api-path-slug: restmethodflickr-stats-getphotodomains-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: date
        description: Stats will be returned for this date
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of domains to return per page
      - in: query
        name: photo_id
        description: The id of the photo to get stats for
      responses:
        200:
          description: OK
      tags:
      - Stats
      - GetPhotoDomains
  /rest/?method=flickr.stats.getPhotoReferrers:
    get:
      summary: Stats Get Photo Referrers
      description: Get a list of referring domains for a photo.
      operationId: getRestMethodFlickr.stats.getphotoreferrers
      x-api-path-slug: restmethodflickr-stats-getphotoreferrers-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: domain
        description: The domain to return referrers for
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of domains to return per page
      - in: query
        name: photo_id
        description: The id of the photo to get stats for
      responses:
        200:
          description: OK
      tags:
      - Stats
      - GetPhotoReferrers
  /rest/?method=flickr.stats.getPhotoStats:
    get:
      summary: Stats Get Photo Stats
      description: Get the number of views, comments and favorites on a photo for
        a given date.
      operationId: getRestMethodFlickr.stats.getphotostats
      x-api-path-slug: restmethodflickr-stats-getphotostats-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: date
        description: Stats will be returned for this date
      - in: query
        name: format
        description: Response format
      - in: query
        name: photo_id
        description: The id of the photo to get stats for
      responses:
        200:
          description: OK
      tags:
      - Stats
      - GetPhotoStats
  /rest/?method=flickr.stats.getPhotosetDomains:
    get:
      summary: Stats Get Photoset Domains
      description: Get a list of referring domains for a photoset.
      operationId: getRestMethodFlickr.stats.getphotosetdomains
      x-api-path-slug: restmethodflickr-stats-getphotosetdomains-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: date
        description: Stats will be returned for this date
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of domains to return per page
      - in: query
        name: photoset_id
        description: The id of the photoset to get stats for
      responses:
        200:
          description: OK
      tags:
      - Stats
      - GetPhotosetDomains
  /rest/?method=flickr.stats.getPhotosetReferrers:
    get:
      summary: Stats Get Photoset Referrers
      description: Get a list of referring domains for a photoset.
      operationId: getRestMethodFlickr.stats.getphotosetreferrers
      x-api-path-slug: restmethodflickr-stats-getphotosetreferrers-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: domain
        description: The domain to return referrers for
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of domains to return per page
      - in: query
        name: photoset_id
        description: The id of the photoset to get stats for
      responses:
        200:
          description: OK
      tags:
      - Stats
      - GetPhotosetReferrers
  /rest/?method=flickr.stats.getPhotosetStats:
    get:
      summary: Stats Get Photoset Stats
      description: Get the number of views on a photoset for a given date.
      operationId: getRestMethodFlickr.stats.getphotosetstats
      x-api-path-slug: restmethodflickr-stats-getphotosetstats-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: date
        description: Stats will be returned for this date
      - in: query
        name: format
        description: Response format
      - in: query
        name: photoset_id
        description: The id of the photoset to get stats for
      responses:
        200:
          description: OK
      tags:
      - Stats
      - GetPhotosetStats
  /rest/?method=flickr.stats.getPhotostreamDomains:
    get:
      summary: Stats Get Photostream Domains
      description: Get a list of referring domains for a photostream.
      operationId: getRestMethodFlickr.stats.getphotostreamdomains
      x-api-path-slug: restmethodflickr-stats-getphotostreamdomains-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: date
        description: Stats will be returned for this date
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of domains to return per page
      responses:
        200:
          description: OK
      tags:
      - Stats
      - GetPhotostreamDomains
  /rest/?method=flickr.stats.getPhotostreamReferrers:
    get:
      summary: Stats Get Photostream Referrers
      description: Get a list of referrers from a given domain to a user's photostream
      operationId: getRestMethodFlickr.stats.getphotostreamreferrers
      x-api-path-slug: restmethodflickr-stats-getphotostreamreferrers-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: domain
        description: The domain to return referrers for
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of domains to return per page
      responses:
        200:
          description: OK
      tags:
      - Stats
      - GetPhotostreamReferrers
  /rest/?method=flickr.stats.getPhotostreamStats:
    get:
      summary: Stats Get Photostream Stats
      description: Get the number of views on a user's photostream for a given date.
      operationId: getRestMethodFlickr.stats.getphotostreamstats
      x-api-path-slug: restmethodflickr-stats-getphotostreamstats-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: date
        description: Stats will be returned for this date
      - in: query
        name: format
        description: Response format
      responses:
        200:
          description: OK
      tags:
      - Stats
      - GetPhotostreamStats
  /rest/?method=flickr.stats.getPopularPhotos:
    get:
      summary: Stats Get Popular Photos
      description: List the photos with the most views, comments or favorites.
      operationId: getRestMethodFlickr.stats.getpopularphotos
      x-api-path-slug: restmethodflickr-stats-getpopularphotos-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: date
        description: Stats will be returned for this date
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of domains to return per page
      - in: query
        name: sort
        description: The order in which to sort returned photos
      responses:
        200:
          description: OK
      tags:
      - Stats
      - GetPopularPhotos
  /rest/?method=flickr.stats.getTotalViews:
    get:
      summary: Stats Get Total Views
      description: Get the overall view counts for an account.
      operationId: getRestMethodFlickr.stats.gettotalviews
      x-api-path-slug: restmethodflickr-stats-gettotalviews-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: date
        description: Stats will be returned for this date
      - in: query
        name: format
        description: Response format
      responses:
        200:
          description: OK
      tags:
      - Stats
      - GetTotalViews
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