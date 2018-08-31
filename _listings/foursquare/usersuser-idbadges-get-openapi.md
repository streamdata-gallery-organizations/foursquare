---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 0
info:
  title: Foursquare Get Users Badges
  description: users/search (POST)
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
  /events/search:
    get:
      summary: Get Events Search
      description: /events/categories
      operationId: eventscategories
      x-api-path-slug: eventssearch-get
      parameters:
      - in: query
        name: domain
        description: Identifier for a known third-party event provider
      - in: query
        name: eventId
        description: Identifier used by third-party specifed in domain, which we will
          attempt to match against our events listings
      - in: query
        name: participantId
        description: Identifier used by third-party specifed in domain, which we will
          attempt to match against our events listings
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Events
      - Search
  /events/{EVENT_ID}:
    get:
      summary: Get Events Event
      description: /campaigns/{CAMPAIGN_ID}/start
      operationId: campaignscampaign-idstart
      x-api-path-slug: eventsevent-id-get
      parameters:
      - in: query
        name: EVENT_ID
        description: The ID of the event to retrieve additional information for
      - in: path
        name: EVENT_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Events
      - Event
  /lists/add:
    post:
      summary: Post Lists Add
      description: /lists/{LIST_ID}
      operationId: listslist-id
      x-api-path-slug: listsadd-post
      parameters:
      - in: query
        name: collaborative
        description: Indicating if this list can be edited by friends
      - in: query
        name: description
        description: The description of the list
      - in: query
        name: name
        description: The name of the list
      - in: query
        name: photoId
        description: The id of a photo that should be set as the list photo
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
  /lists/{LIST_ID}:
    get:
      summary: Get Lists
      description: /tips/{TIP_ID}/unmark
      operationId: tipstip-idunmark
      x-api-path-slug: listslist-id-get
      parameters:
      - in: query
        name: limit
        description: Number of results to return, up to 200
      - in: query
        name: LIST_ID
        description: id for a user-created (e
      - in: path
        name: LIST_ID
      - in: query
        name: offset
        description: The number of results to skip
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
  /lists/{LIST_ID}/additem:
    post:
      summary: Post Lists Additem
      description: /lists/{LIST_ID}/suggestvenues
      operationId: listslist-idsuggestvenues
      x-api-path-slug: listslist-idadditem-post
      parameters:
      - in: query
        name: itemId
        description: Used in conjuction with listId, the id of an item on that list
          that we wish to copy to this list
      - in: query
        name: listId
        description: Used in conjuction with itemId, the id for a user created or
          followed list as well as one of USER_ID/tips, USER_ID/todos, or USER_ID/dones
      - in: query
        name: LIST_ID
        description: Id for a user-created or followed list as well as one of USER_ID/tips,
          USER_ID/todos, or USER_ID/dones
      - in: path
        name: LIST_ID
      - in: query
        name: text
        description: If the target is a user-created list, this will create a public
          tip on the venue
      - in: query
        name: tipId
        description: Used to add a tip to a list
      - in: query
        name: url
        description: If adding a new tip via text, this can associate a url with the
          tip
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: venueId
        description: A venue to add to the list
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Item
  /lists/{LIST_ID}/deleteitem:
    post:
      summary: Post Lists Deleteitem
      description: /lists/{LIST_ID}/additem
      operationId: listslist-idadditem
      x-api-path-slug: listslist-iddeleteitem-post
      parameters:
      - in: query
        name: itemId
        description: Id of the item to delete
      - in: query
        name: LIST_ID
        description: Id for a user-created or followed list or one of USER_ID/tips,
          USER_ID/todos, or USER_ID/dones
      - in: path
        name: LIST_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Item
  /lists/{LIST_ID}/follow:
    post:
      summary: Post Lists Follow
      description: /lists/{LIST_ID}/deleteitem
      operationId: listslist-iddeleteitem
      x-api-path-slug: listslist-idfollow-post
      parameters:
      - in: query
        name: LIST_ID
        description: Id of a user-created list
      - in: path
        name: LIST_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Follow
  /lists/{LIST_ID}/followers:
    get:
      summary: Get Lists Followers
      description: /lists/add
      operationId: listsadd
      x-api-path-slug: listslist-idfollowers-get
      parameters:
      - in: query
        name: LIST_ID
        description: Id for a user-created list
      - in: path
        name: LIST_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Followers
  /lists/{LIST_ID}/moveitem:
    post:
      summary: Post Lists Moveitem
      description: /lists/{LIST_ID}/follow
      operationId: listslist-idfollow
      x-api-path-slug: listslist-idmoveitem-post
      parameters:
      - in: query
        name: afterId
        description: Move itemId after afterId
      - in: query
        name: beforeId
        description: Move itemId before beforeId
      - in: query
        name: itemId
        description: Id of the item on this list to move
      - in: query
        name: LIST_ID
        description: Id for a user-created or followed list or one of USER_ID/tips,
          USER_ID/todos, or USER_ID/dones
      - in: path
        name: LIST_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Moveitem
  /lists/{LIST_ID}/share:
    post:
      summary: Post Lists Share
      description: /lists/{LIST_ID}/moveitem
      operationId: listslist-idmoveitem
      x-api-path-slug: listslist-idshare-post
      parameters:
      - in: query
        name: broadcast
        description: Where to broadcast this list
      - in: query
        name: LIST_ID
        description: Id for a user-created list
      - in: path
        name: LIST_ID
      - in: query
        name: message
        description: A personal note to include with the share
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Share
  /lists/{LIST_ID}/suggestphoto:
    get:
      summary: Get Lists Suggestphoto
      description: /lists/{LIST_ID}/followers
      operationId: listslist-idfollowers
      x-api-path-slug: listslist-idsuggestphoto-get
      parameters:
      - in: query
        name: itemId
        description: Id of item on this list
      - in: query
        name: LIST_ID
        description: Id for a user-created list
      - in: path
        name: LIST_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Suggestphoto
  /lists/{LIST_ID}/suggesttip:
    get:
      summary: Get Lists Suggesttip
      description: /lists/{LIST_ID}/suggestphoto
      operationId: listslist-idsuggestphoto
      x-api-path-slug: listslist-idsuggesttip-get
      parameters:
      - in: query
        name: itemId
        description: Id of item on this list
      - in: query
        name: LIST_ID
        description: Id for a user-created list
      - in: path
        name: LIST_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Suggesttip
  /lists/{LIST_ID}/suggestvenues:
    get:
      summary: Get Lists Suggestvenues
      description: /lists/{LIST_ID}/suggesttip
      operationId: listslist-idsuggesttip
      x-api-path-slug: listslist-idsuggestvenues-get
      parameters:
      - in: query
        name: LIST_ID
        description: Id for a user-created list
      - in: path
        name: LIST_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Suggestvenues
  /lists/{LIST_ID}/unfollow:
    post:
      summary: Post Lists Unfollow
      description: /lists/{LIST_ID}/share
      operationId: listslist-idshare
      x-api-path-slug: listslist-idunfollow-post
      parameters:
      - in: query
        name: LIST_ID
        description: Id of a user-created list
      - in: path
        name: LIST_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Unfollow
  /lists/{LIST_ID}/update:
    post:
      summary: Post Lists Update
      description: /lists/{LIST_ID}/unfollow
      operationId: listslist-idunfollow
      x-api-path-slug: listslist-idupdate-post
      parameters:
      - in: query
        name: collaborative
        description: Indicating if this list can be edited by friends
      - in: query
        name: description
        description: If present and a non-empty value, updates the List description
      - in: query
        name: LIST_ID
        description: Id for a user-created list
      - in: path
        name: LIST_ID
      - in: query
        name: name
        description: If present and a non-empty value, updates the List name
      - in: query
        name: photoId
        description: If present and a non-empty value, updates the List photo
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
  /lists/{LIST_ID}/updateitem:
    post:
      summary: Post Lists Updateitem
      description: /lists/{LIST_ID}/update
      operationId: listslist-idupdate
      x-api-path-slug: listslist-idupdateitem-post
      parameters:
      - in: query
        name: itemId
        description: The id of an item on this list
      - in: query
        name: LIST_ID
        description: Id for a user-created list
      - in: path
        name: LIST_ID
      - in: query
        name: photoId
        description: If present and a non-empty value, adds a photo to this item
      - in: query
        name: text
        description: If present creates a public tip on the venue and replaces any
          existing tip on the item
      - in: query
        name: tipId
        description: If present and a non-empty value, adds or replaces a tip on this
          item
      - in: query
        name: url
        description: If adding a new tip via text, this can associate a url with the
          tip
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Item
  /multi:
    get:
      summary: Get Multi
      description: /pages/{PAGE_ID}/venues
      operationId: pagespage-idvenues
      x-api-path-slug: multi-get
      parameters:
      - in: query
        name: requests
        description: A comma-delimited list of API requests
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Multi
  /pages/search:
    get:
      summary: Get Pages Search
      description: /pages/{PAGE_ID}
      operationId: pagespage-id
      x-api-path-slug: pagessearch-get
      parameters:
      - in: query
        name: fbid
        description: A comma-delimited list of Facebook IDs to look for
      - in: query
        name: name
        description: A search term to be applied against page names
      - in: query
        name: twitter
        description: A comma-delimited list of Twitter handles to look for
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Pages
      - Search
  /pages/{PAGE_ID}:
    get:
      summary: Get Pages
      description: /events/search
      operationId: eventssearch
      x-api-path-slug: pagespage-id-get
      parameters:
      - in: query
        name: PAGE_ID
        description: Identity of the page to get details for
      - in: path
        name: PAGE_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Pages
  /pages/{PAGE_ID}/venues:
    get:
      summary: Get Pages Venues
      description: /pages/search
      operationId: pagessearch
      x-api-path-slug: pagespage-idvenues-get
      parameters:
      - in: query
        name: limit
        description: The number of venues to return
      - in: query
        name: ll
        description: Not valid with ne or sw
      - in: query
        name: ne
        description: See sw
      - in: query
        name: offset
        description: The offset of which venues to return
      - in: query
        name: PAGE_ID
        description: The page id for which venues are being requested
      - in: path
        name: PAGE_ID
      - in: query
        name: radius
        description: Can be used when including ll
      - in: query
        name: sw
        description: With ne, limits results to the bounding quadrangle defined by
          the latitude and longitude given by sw as its south-west corner, and ne
          as its north-east corner
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Pages
      - Venues
  /photos/add:
    post:
      summary: Post Photos Add
      description: /photos/{PHOTO_ID}
      operationId: photosphoto-id
      x-api-path-slug: photosadd-post
      parameters:
      - in: query
        name: alt
        description: Altitude of the users location, in meters
      - in: query
        name: altAcc
        description: Vertical accuracy of the users location, in meters
      - in: query
        name: broadcast
        description: Whether to broadcast this photo
      - in: query
        name: checkinId
        description: The ID of a checkin owned by the user
      - in: query
        name: Content-Type
        description: Content-Type
      - in: query
        name: image
        description: The image file data
      - in: query
        name: ll
        description: Latitude and longitude of the users location
      - in: query
        name: llAcc
        description: Accuracy of the users latitude and longitude, in meters
      - in: query
        name: public
        description: When the checkinId is also provided (meaning this is a photo
          attached to a checkin), this parameter allows for making the photo public
          and viewable at the venue
      - in: query
        name: tipId
        description: The ID of a tip owned by the user
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: venueId
        description: The ID of a venue, provided only when adding a public photo of
          the venue in general, rather than a private checkin or tip photo using the
          parameters above
      responses:
        200:
          description: OK
      tags:
      - Photos
  /photos/{PHOTO_ID}:
    get:
      summary: Get Photos Photo
      description: /updates/marknotificationsread
      operationId: updatesmarknotificationsread
      x-api-path-slug: photosphoto-id-get
      parameters:
      - in: query
        name: PHOTO_ID
        description: The ID of the photo to retrieve additional information for
      - in: path
        name: PHOTO_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Photo
  /settings/all:
    get:
      summary: Get Settings All
      description: /settings/{SETTING_ID}
      operationId: settingssetting-id
      x-api-path-slug: settingsall-get
      parameters:
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Settings
  /settings/{SETTING_ID}:
    get:
      summary: Get Settings Setting
      description: /photos/add
      operationId: photosadd
      x-api-path-slug: settingssetting-id-get
      parameters:
      - in: query
        name: SETTING_ID
        description: The name of a setting
      - in: path
        name: SETTING_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Settings
      - Setting
  /settings/{SETTING_ID}/set:
    post:
      summary: Post Settings Setting Set
      description: /settings/all
      operationId: settingsall
      x-api-path-slug: settingssetting-idset-post
      parameters:
      - in: query
        name: SETTING_ID
        description: Name of setting to change
      - in: path
        name: SETTING_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: value
        description: 1 for true, and 0 for false
      responses:
        200:
          description: OK
      tags:
      - Settings
      - Setting
      - Set
  /specials/add:
    post:
      summary: Post Specials Add
      description: /specials/{SPECIAL_ID}
      operationId: specialsspecial-id
      x-api-path-slug: specialsadd-post
      parameters:
      - in: query
        name: cost
        description: The amount of money the user must spend to use this special in
          dollars and cents
      - in: query
        name: count1
        description: Count for frequency, count, regular, swarm, friends, and flash
          specials
      - in: query
        name: count2
        description: Secondary count for regular, flash specials
      - in: query
        name: count3
        description: Tertiary count for flash specials
      - in: query
        name: finePrint
        description: Maximum length of 200 characters
      - in: query
        name: name
        description: A name for the special
      - in: query
        name: offerId
        description: Maximum length of 16 characters
      - in: query
        name: text
        description: Maximum length of 200 characters
      - in: query
        name: type
        description: The type of special
      - in: query
        name: unlockedText
        description: Maximum length of 200 characters
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Specials
  /specials/list:
    get:
      summary: Get Specials List
      description: /specials/add
      operationId: specialsadd
      x-api-path-slug: specialslist-get
      parameters:
      - in: query
        name: status
        description: 'Which specials to return: pending, active, expired, all'
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: venueId
        description: Comma-separated list of venue IDs; filters results to the specials
          assigned to the venue(s)
      responses:
        200:
          description: OK
      tags:
      - Specials
      - List
  /specials/search:
    get:
      summary: Get Specials Search
      description: /specials/list
      operationId: specialslist
      x-api-path-slug: specialssearch-get
      parameters:
      - in: query
        name: alt
        description: Altitude of the users location, in meters
      - in: query
        name: altAcc
        description: Accuracy of the users altitude, in meters
      - in: query
        name: limit
        description: Number of results to return, up to 50
      - in: query
        name: ll
        description: Latitude and longitude to search near
      - in: query
        name: llAcc
        description: Accuracy of latitude and longitude, in meters
      - in: query
        name: radius
        description: Limit results to venues within this many meters of the specified
          location
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Specials
      - Search
  /specials/{ID}/flag:
    post:
      summary: Post Specials Flag
      description: /specials/{SPECIAL_ID}/configuration
      operationId: specialsspecial-idconfiguration
      x-api-path-slug: specialsidflag-post
      parameters:
      - in: query
        name: ID
        description: The id of the special being flagged
      - in: path
        name: ID
      - in: query
        name: problem
        description: One of not_redeemable, not_valuable, other
      - in: query
        name: text
        description: Additional text about why the user has flagged this special
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: venueId
        description: The id of the venue running the special
      responses:
        200:
          description: OK
      tags:
      - Specials
      - Flag
  /specials/{SPECIAL_ID}:
    get:
      summary: Get Specials
      description: /settings/{SETTING_ID}/set
      operationId: settingssetting-idset
      x-api-path-slug: specialsspecial-id-get
      parameters:
      - in: query
        name: SPECIAL_ID
        description: ID of special to retrieve
      - in: path
        name: SPECIAL_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: venueId
        description: ID of a venue the special is running at
      responses:
        200:
          description: OK
      tags:
      - Specials
  /specials/{SPECIAL_ID}/configuration:
    get:
      summary: Get Specials Configuration
      description: /specials/search
      operationId: specialssearch
      x-api-path-slug: specialsspecial-idconfiguration-get
      parameters:
      - in: query
        name: SPECIAL_ID
        description: The ID of the special to retrieve configuration details for
      - in: path
        name: SPECIAL_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Specials
      - Configuration
  /specials/{SPECIAL_ID}/retire:
    post:
      summary: Post Specials Retire
      description: /specials/{ID}/flag
      operationId: specialsidflag
      x-api-path-slug: specialsspecial-idretire-post
      parameters:
      - in: query
        name: SPECIAL_ID
        description: The ID of the special to retire
      - in: path
        name: SPECIAL_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Specials
      - Retire
  /tips/add:
    post:
      summary: Post Tips Add
      description: /tips/{TIP_ID}
      operationId: tipstip-id
      x-api-path-slug: tipsadd-post
      parameters:
      - in: query
        name: broadcast
        description: Whether to broadcast this tip
      - in: query
        name: text
        description: The text of the tip, up to 200 characters
      - in: query
        name: url
        description: A URL related to this tip
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: venueId
        description: The venue where you want to add this tip
      responses:
        200:
          description: OK
      tags:
      - Tips
  /tips/search:
    get:
      summary: Get Tips Search
      description: /tips/add
      operationId: tipsadd
      x-api-path-slug: tipssearch-get
      parameters:
      - in: query
        name: filter
        description: If set to friends, only show nearby tips from friends
      - in: query
        name: limit
        description: Number of results to return, up to 500
      - in: query
        name: ll
        description: Latitude and longitude of the users location
      - in: query
        name: offset
        description: Used to page through results
      - in: query
        name: query
        description: Only find tips matching the given term, cannot be used in conjunction
          with friends filter
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Tips
      - Search
  /tips/{TIP_ID}:
    get:
      summary: Get Tips
      description: /checkins/{CHECKIN_ID}/deletecomment
      operationId: checkinscheckin-iddeletecomment
      x-api-path-slug: tipstip-id-get
      parameters:
      - in: query
        name: TIP_ID
        description: ID of tip to retrieve
      - in: path
        name: TIP_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Tips
  /tips/{TIP_ID}/done:
    get:
      summary: Get Tips Done
      description: /tips/search
      operationId: tipssearch
      x-api-path-slug: tipstip-iddone-get
      parameters:
      - in: query
        name: limit
        description: Number of results to return, up to 200
      - in: query
        name: offset
        description: Used to page through results
      - in: query
        name: TIP_ID
        description: Identity of a tip to get users who have marked the tip as done
      - in: path
        name: TIP_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Tips
      - Done
  /tips/{TIP_ID}/listed:
    get:
      summary: Get Tips Listed
      description: /tips/{TIP_ID}/done
      operationId: tipstip-iddone
      x-api-path-slug: tipstip-idlisted-get
      parameters:
      - in: query
        name: group
        description: Can be created, edited, followed, friends, other
      - in: query
        name: TIP_ID
        description: Identity of a tip to get lists for
      - in: path
        name: TIP_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Tips
      - Listed
  /tips/{TIP_ID}/markdone:
    post:
      summary: Post Tips Markdone
      description: /tips/{TIP_ID}/listed
      operationId: tipstip-idlisted
      x-api-path-slug: tipstip-idmarkdone-post
      parameters:
      - in: query
        name: TIP_ID
        description: The tip you want to mark done
      - in: path
        name: TIP_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Tips
      - Markdone
  /tips/{TIP_ID}/marktodo:
    post:
      summary: Post Tips Marktodo
      description: /tips/{TIP_ID}/markdone
      operationId: tipstip-idmarkdone
      x-api-path-slug: tipstip-idmarktodo-post
      parameters:
      - in: query
        name: TIP_ID
        description: The tip you want to mark to-do
      - in: path
        name: TIP_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Tips
      - Marktodo
  /tips/{TIP_ID}/unmark:
    post:
      summary: Post Tips Unmark
      description: /tips/{TIP_ID}/marktodo
      operationId: tipstip-idmarktodo
      x-api-path-slug: tipstip-idunmark-post
      parameters:
      - in: query
        name: TIP_ID
        description: The tip you want to unmark
      - in: path
        name: TIP_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Tips
      - Unmark
  /updates/marknotificationsread:
    post:
      summary: Post Updates Marknotificationsread
      description: /updates/notifications
      operationId: updatesnotifications
      x-api-path-slug: updatesmarknotificationsread-post
      parameters:
      - in: query
        name: highWatermark
        description: The timestamp of the most recent notification that the user viewed
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - S
      - Marknotificationsread
  /updates/notifications:
    get:
      summary: Get Updates Notifications
      description: /updates/{UPDATE_ID}
      operationId: updatesupdate-id
      x-api-path-slug: updatesnotifications-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of results to return, up to 99
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - S
      - Notifications
  /updates/{UPDATE_ID}:
    get:
      summary: Get Updates Update
      description: /lists/{LIST_ID}/updateitem
      operationId: listslist-idupdateitem
      x-api-path-slug: updatesupdate-id-get
      parameters:
      - in: query
        name: UPDATE_ID
        description: The ID of the update to retrieve
      - in: path
        name: UPDATE_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - S
  /users/leaderboard:
    get:
      summary: Get Users Leaderboard
      description: /users/{USER_ID}
      operationId: usersuser-id
      x-api-path-slug: usersleaderboard-get
      parameters:
      - in: query
        name: neighbors
        description: Number of friends scores to return that are adjacent to your
          score, in ranked order
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Leaderboard
  /users/requests:
    get:
      summary: Get Users Requests
      description: /users/leaderboard
      operationId: usersleaderboard
      x-api-path-slug: usersrequests-get
      parameters:
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Requests
  /users/search:
    get:
      summary: Get Users Search
      description: /users/requests
      operationId: usersrequests
      x-api-path-slug: userssearch-get
      parameters:
      - in: query
        name: email
        description: A comma-delimited list of email addresses to look for
      - in: query
        name: fbid
        description: A comma-delimited list of Facebook IDs to look for
      - in: query
        name: name
        description: A single string to search for in users names
      - in: query
        name: phone
        description: A comma-delimited list of phone numbers to look for
      - in: query
        name: twitter
        description: A comma-delimited list of Twitter handles to look for
      - in: query
        name: twitterSource
        description: A single Twitter handle
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Search
    post:
      summary: Post Users Search
      description: users/search (GET)
      operationId: userssearch-get
      x-api-path-slug: userssearch-post
      parameters:
      - in: query
        name: email
        description: A comma-delimited list of email addresses to look for
      - in: query
        name: fbid
        description: A comma-delimited list of Facebook IDs to look for
      - in: query
        name: name
        description: A single string to search for in users names
      - in: query
        name: phone
        description: A comma-delimited list of phone numbers to look for
      - in: query
        name: twitter
        description: A comma-delimited list of Twitter handles to look for
      - in: query
        name: twitterSource
        description: A single Twitter handle
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Search
  /users/self/update:
    post:
      summary: Post Users Self Update
      description: /users/{USER_ID}/unfriend
      operationId: usersuser-idunfriend
      x-api-path-slug: usersselfupdate-post
      parameters:
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: photo
        description: Photo under 100KB in multipart MIME encoding with content type
          image/jpeg, image/gif, or image/png
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
  /users/{USER_ID}:
    get:
      summary: Get Users
      description: ""
      operationId: ""
      x-api-path-slug: usersuser-id-get
      parameters:
      - in: query
        name: USER_ID
        description: Identity of the user to get details for
      - in: path
        name: USER_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{USER_ID}/approve:
    post:
      summary: Post Users Approve
      description: /users/{USER_ID}/venuehistory
      operationId: usersuser-idvenuehistory
      x-api-path-slug: usersuser-idapprove-post
      parameters:
      - in: query
        name: USER_ID
        description: The user ID of a pending friend
      - in: path
        name: USER_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Approve
  /users/{USER_ID}/badges:
    get:
      summary: Get Users Badges
      description: users/search (POST)
      operationId: userssearch-post
      x-api-path-slug: usersuser-idbadges-get
      parameters:
      - in: query
        name: USER_ID
        description: ID for user to view badges for
      - in: path
        name: USER_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Badges
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