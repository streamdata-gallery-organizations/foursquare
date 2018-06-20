---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 0
info:
  title: Foursquare Post Campaigns Add
  description: /campaigns/{CAMPAIGN_ID}
  version: 1.0.0
host: api.foursquare.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /campaigns/add:
    post:
      summary: Post Campaigns Add
      description: /campaigns/{CAMPAIGN_ID}
      operationId: campaignscampaign-id
      x-api-path-slug: campaignsadd-post
      parameters:
      - in: query
        name: campaignId
        description: ID of an existing campaign to copy
      - in: query
        name: endAt
        description: DateTime when the campaign is to be automatically deactivated
          (seconds since epoch)
      - in: query
        name: groupId
        description: required (unless venueId has been provided)
      - in: query
        name: specialId
        description: required (unless campaignId has been provided)
      - in: query
        name: startAt
        description: DateTime when the campaign is to be started (seconds since epoch)
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: venueId
        description: required (unless groupId has been provided)
      responses:
        200:
          description: OK
      tags:
      - Campaigns
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