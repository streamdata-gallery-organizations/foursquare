---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 0
info:
  title: Foursquare Post Campaigns Delete
  description: /campaigns/{CAMPAIGN_ID}/timeseries
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
  /campaigns/list:
    get:
      summary: Get Campaigns List
      description: /campaigns/add
      operationId: campaignsadd
      x-api-path-slug: campaignslist-get
      parameters:
      - in: query
        name: groupId
        description: If specified, limits response to campaigns involving the given
          group
      - in: query
        name: specialId
        description: If specified, limits response to campaigns involving the given
          special
      - in: query
        name: status
        description: 'Which campaigns to return: pending, active, expired, all (default=all)'
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - List
  /campaigns/{CAMPAIGN_ID}:
    get:
      summary: Get Campaigns
      description: /specials/{SPECIAL_ID}/retire
      operationId: specialsspecial-idretire
      x-api-path-slug: campaignscampaign-id-get
      parameters:
      - in: query
        name: CAMPAIGN_ID
        description: The ID of the campaign to retrieve additional information for
      - in: path
        name: CAMPAIGN_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Campaigns
  /campaigns/{CAMPAIGN_ID}/delete:
    post:
      summary: Post Campaigns Delete
      description: /campaigns/{CAMPAIGN_ID}/timeseries
      operationId: campaignscampaign-idtimeseries
      x-api-path-slug: campaignscampaign-iddelete-post
      parameters:
      - in: query
        name: CAMPAIGN_ID
        description: The ID of the campaign to delete
      - in: path
        name: CAMPAIGN_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
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