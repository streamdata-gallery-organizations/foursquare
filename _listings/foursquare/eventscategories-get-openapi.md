---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 0
info:
  title: Foursquare Get Events Categories
  description: /events/{EVENT_ID}
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
  /campaigns/{CAMPAIGN_ID}/end:
    post:
      summary: Post Campaigns End
      description: /campaigns/{CAMPAIGN_ID}/delete
      operationId: campaignscampaign-iddelete
      x-api-path-slug: campaignscampaign-idend-post
      parameters:
      - in: query
        name: CAMPAIGN_ID
        description: The ID of the campaign to end
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
      - End
  /campaigns/{CAMPAIGN_ID}/start:
    post:
      summary: Post Campaigns Start
      description: /campaigns/{CAMPAIGN_ID}/end
      operationId: campaignscampaign-idend
      x-api-path-slug: campaignscampaign-idstart-post
      parameters:
      - in: query
        name: CAMPAIGN_ID
        description: The ID of the campaign to start
      - in: path
        name: CAMPAIGN_ID
      - in: query
        name: startAt
        description: DateTime when the campaign is to be started (seconds since epoch)
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - Start
  /campaigns/{CAMPAIGN_ID}/timeseries:
    get:
      summary: Get Campaigns Timeseries
      description: /campaigns/list
      operationId: campaignslist
      x-api-path-slug: campaignscampaign-idtimeseries-get
      parameters:
      - in: query
        name: CAMPAIGN_ID
        description: The campaign id to retrieve stats for
      - in: path
        name: CAMPAIGN_ID
      - in: query
        name: endAt
        description: The end of the time range to retrieve stats for (seconds since
          epoch)
      - in: query
        name: startAt
        description: The start of the time range to retrieve stats for (seconds since
          epoch)
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - Timeseries
  /checkins/add:
    post:
      summary: Post Checkins Add
      description: /checkins/{CHECKIN_ID}
      operationId: checkinscheckin-id
      x-api-path-slug: checkinsadd-post
      parameters:
      - in: query
        name: alt
        description: Altitude of the users location, in meters
      - in: query
        name: altAcc
        description: Vertical accuracy of the users location, in meters
      - in: query
        name: broadcast
        description: Who to broadcast this check-in to
      - in: query
        name: eventId
        description: The event the user is checking in to
      - in: query
        name: ll
        description: Latitude and longitude of the users location
      - in: query
        name: llAcc
        description: Accuracy of the users latitude and longitude, in meters
      - in: query
        name: shout
        description: A message about your check-in
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: venue
        description: If are not shouting, but you dont have a venue ID or would rather
          prefer a venueless checkin, pass the venue name as a string using this parameter
      - in: query
        name: venueId
        description: The venue where the user is checking in
      responses:
        200:
          description: OK
      tags:
      - Checkins
  /checkins/recent:
    get:
      summary: Get Checkins Recent
      description: /checkins/add
      operationId: checkinsadd
      x-api-path-slug: checkinsrecent-get
      parameters:
      - in: query
        name: afterTimestamp
        description: Seconds after which to look for checkins, e
      - in: query
        name: limit
        description: Number of results to return, up to 100
      - in: query
        name: ll
        description: Latitude and longitude of the users location, so response can
          include distance
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Checkins
      - Recent
  /checkins/{CHECKIN_ID}:
    get:
      summary: Get Checkins Checkin
      description: /venuegroups/{GROUP_ID}/removevenue
      operationId: venuegroupsgroup-idremovevenue
      x-api-path-slug: checkinscheckin-id-get
      parameters:
      - in: query
        name: CHECKIN_ID
        description: The ID of the checkin to retrieve additional information for
      - in: path
        name: CHECKIN_ID
      - in: query
        name: signature
        description: When checkins are sent to public feeds such as Twitter, foursquare
          appends a signature (s=XXXXXX) allowing users to bypass the friends-only
          access check on checkins
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Checkins
      - Checkin
  /checkins/{CHECKIN_ID}/addcomment:
    post:
      summary: Post Checkins Checkin Addcomment
      description: /checkins/recent
      operationId: checkinsrecent
      x-api-path-slug: checkinscheckin-idaddcomment-post
      parameters:
      - in: query
        name: CHECKIN_ID
        description: The ID of the checkin to add a comment to
      - in: path
        name: CHECKIN_ID
      - in: query
        name: text
        description: The text of the comment, up to 200 characters
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Checkins
      - Checkin
      - Comment
  /checkins/{CHECKIN_ID}/deletecomment:
    post:
      summary: Post Checkins Checkin Deletecomment
      description: /checkins/{CHECKIN_ID}/addcomment
      operationId: checkinscheckin-idaddcomment
      x-api-path-slug: checkinscheckin-iddeletecomment-post
      parameters:
      - in: query
        name: CHECKIN_ID
        description: The ID of the checkin to remove a comment from
      - in: path
        name: CHECKIN_ID
      - in: query
        name: commentId
        description: The id of the comment to remove
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Checkins
      - Checkin
      - Comment
  /events/categories:
    get:
      summary: Get Events Categories
      description: /events/{EVENT_ID}
      operationId: eventsevent-id
      x-api-path-slug: eventscategories-get
      parameters:
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Events
      - Categories
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