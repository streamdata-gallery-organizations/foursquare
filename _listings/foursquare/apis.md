---
name: Foursquare
x-slug: foursquare
description: Foursquare helps you find the perfect places to go with friends. Discover
  the best food, nightlife, and entertainment in your area.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
x-kinRank: "9"
x-alexaRank: "2544"
tags: Foursquare
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/apis.md
specificationVersion: "0.14"
apis:
- name: Foursquare Post Campaigns Add
  x-api-slug: foursquare
  description: /campaigns/{CAMPAIGN_ID}
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///campaigns/add
  tags: Campaigns
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/campaignsadd-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/campaignsadd-post-openapi.md
- name: Foursquare Get Campaigns List
  x-api-slug: foursquare
  description: /campaigns/add
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///campaigns/list
  tags: Campaigns,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/campaignslist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/campaignslist-get-openapi.md
- name: Foursquare Get Campaigns
  x-api-slug: foursquare
  description: /specials/{SPECIAL_ID}/retire
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///campaigns/{CAMPAIGN_ID}
  tags: Campaigns
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/campaignscampaign-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/campaignscampaign-id-get-openapi.md
- name: Foursquare Post Campaigns Delete
  x-api-slug: foursquare
  description: /campaigns/{CAMPAIGN_ID}/timeseries
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///campaigns/{CAMPAIGN_ID}/delete
  tags: Campaigns
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/campaignscampaign-iddelete-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/campaignscampaign-iddelete-post-openapi.md
- name: Foursquare Post Campaigns End
  x-api-slug: foursquare
  description: /campaigns/{CAMPAIGN_ID}/delete
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///campaigns/{CAMPAIGN_ID}/end
  tags: Campaigns,End
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/campaignscampaign-idend-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/campaignscampaign-idend-post-openapi.md
- name: Foursquare Post Campaigns Start
  x-api-slug: foursquare
  description: /campaigns/{CAMPAIGN_ID}/end
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///campaigns/{CAMPAIGN_ID}/start
  tags: Campaigns,Start
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/campaignscampaign-idstart-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/campaignscampaign-idstart-post-openapi.md
- name: Foursquare Get Campaigns Timeseries
  x-api-slug: foursquare
  description: /campaigns/list
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///campaigns/{CAMPAIGN_ID}/timeseries
  tags: Campaigns,Timeseries
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/campaignscampaign-idtimeseries-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/campaignscampaign-idtimeseries-get-openapi.md
- name: Foursquare Post Checkins Add
  x-api-slug: foursquare
  description: /checkins/{CHECKIN_ID}
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///checkins/add
  tags: Checkins
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/checkinsadd-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/checkinsadd-post-openapi.md
- name: Foursquare Get Checkins Recent
  x-api-slug: foursquare
  description: /checkins/add
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///checkins/recent
  tags: Checkins,Recent
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/checkinsrecent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/checkinsrecent-get-openapi.md
- name: Foursquare Get Checkins Checkin
  x-api-slug: foursquare
  description: /venuegroups/{GROUP_ID}/removevenue
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///checkins/{CHECKIN_ID}
  tags: Checkins,Checkin
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/checkinscheckin-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/checkinscheckin-id-get-openapi.md
- name: Foursquare Post Checkins Checkin Addcomment
  x-api-slug: foursquare
  description: /checkins/recent
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///checkins/{CHECKIN_ID}/addcomment
  tags: Checkins,Checkin,Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/checkinscheckin-idaddcomment-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/checkinscheckin-idaddcomment-post-openapi.md
- name: Foursquare Post Checkins Checkin Deletecomment
  x-api-slug: foursquare
  description: /checkins/{CHECKIN_ID}/addcomment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///checkins/{CHECKIN_ID}/deletecomment
  tags: Checkins,Checkin,Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/checkinscheckin-iddeletecomment-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/checkinscheckin-iddeletecomment-post-openapi.md
- name: Foursquare Get Events Categories
  x-api-slug: foursquare
  description: /events/{EVENT_ID}
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///events/categories
  tags: Events,Categories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/eventscategories-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/eventscategories-get-openapi.md
- name: Foursquare Get Events Search
  x-api-slug: foursquare
  description: /events/categories
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///events/search
  tags: Events,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/eventssearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/eventssearch-get-openapi.md
- name: Foursquare Get Events Event
  x-api-slug: foursquare
  description: /campaigns/{CAMPAIGN_ID}/start
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///events/{EVENT_ID}
  tags: Events,Event
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/eventsevent-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/eventsevent-id-get-openapi.md
- name: Foursquare Post Lists Add
  x-api-slug: foursquare
  description: /lists/{LIST_ID}
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/add
  tags: Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listsadd-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listsadd-post-openapi.md
- name: Foursquare Get Lists
  x-api-slug: foursquare
  description: /tips/{TIP_ID}/unmark
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}
  tags: Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-id-get-openapi.md
- name: Foursquare Post Lists Additem
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/suggestvenues
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/additem
  tags: Lists,Item
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-idadditem-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-idadditem-post-openapi.md
- name: Foursquare Post Lists Deleteitem
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/additem
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/deleteitem
  tags: Lists,Item
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-iddeleteitem-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-iddeleteitem-post-openapi.md
- name: Foursquare Post Lists Follow
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/deleteitem
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/follow
  tags: Lists,Follow
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-idfollow-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-idfollow-post-openapi.md
- name: Foursquare Get Lists Followers
  x-api-slug: foursquare
  description: /lists/add
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/followers
  tags: Lists,Followers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-idfollowers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-idfollowers-get-openapi.md
- name: Foursquare Post Lists Moveitem
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/follow
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/moveitem
  tags: Lists,Moveitem
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-idmoveitem-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-idmoveitem-post-openapi.md
- name: Foursquare Post Lists Share
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/moveitem
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/share
  tags: Lists,Share
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-idshare-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-idshare-post-openapi.md
- name: Foursquare Get Lists Suggestphoto
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/followers
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/suggestphoto
  tags: Lists,Suggestphoto
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-idsuggestphoto-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-idsuggestphoto-get-openapi.md
- name: Foursquare Get Lists Suggesttip
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/suggestphoto
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/suggesttip
  tags: Lists,Suggesttip
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-idsuggesttip-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-idsuggesttip-get-openapi.md
- name: Foursquare Get Lists Suggestvenues
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/suggesttip
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/suggestvenues
  tags: Lists,Suggestvenues
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-idsuggestvenues-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-idsuggestvenues-get-openapi.md
- name: Foursquare Post Lists Unfollow
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/share
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/unfollow
  tags: Lists,Unfollow
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-idunfollow-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-idunfollow-post-openapi.md
- name: Foursquare Post Lists Update
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/unfollow
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/update
  tags: Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-idupdate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-idupdate-post-openapi.md
- name: Foursquare Post Lists Updateitem
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/update
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/updateitem
  tags: Lists,Item
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-idupdateitem-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/listslist-idupdateitem-post-openapi.md
- name: Foursquare Get Multi
  x-api-slug: foursquare
  description: /pages/{PAGE_ID}/venues
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///multi
  tags: Multi
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/multi-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/multi-get-openapi.md
- name: Foursquare Get Pages Search
  x-api-slug: foursquare
  description: /pages/{PAGE_ID}
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///pages/search
  tags: Pages,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/pagessearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/pagessearch-get-openapi.md
- name: Foursquare Get Pages
  x-api-slug: foursquare
  description: /events/search
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///pages/{PAGE_ID}
  tags: Pages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/pagespage-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/pagespage-id-get-openapi.md
- name: Foursquare Get Pages Venues
  x-api-slug: foursquare
  description: /pages/search
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///pages/{PAGE_ID}/venues
  tags: Pages,Venues
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/pagespage-idvenues-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/pagespage-idvenues-get-openapi.md
- name: Foursquare Post Photos Add
  x-api-slug: foursquare
  description: /photos/{PHOTO_ID}
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///photos/add
  tags: Photos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/photosadd-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/photosadd-post-openapi.md
- name: Foursquare Get Photos Photo
  x-api-slug: foursquare
  description: /updates/marknotificationsread
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///photos/{PHOTO_ID}
  tags: Photos,Photo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/photosphoto-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/photosphoto-id-get-openapi.md
- name: Foursquare Get Settings All
  x-api-slug: foursquare
  description: /settings/{SETTING_ID}
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///settings/all
  tags: Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/settingsall-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/settingsall-get-openapi.md
- name: Foursquare Get Settings Setting
  x-api-slug: foursquare
  description: /photos/add
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///settings/{SETTING_ID}
  tags: Settings,Setting
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/settingssetting-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/settingssetting-id-get-openapi.md
- name: Foursquare Post Settings Setting Set
  x-api-slug: foursquare
  description: /settings/all
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///settings/{SETTING_ID}/set
  tags: Settings,Setting,Set
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/settingssetting-idset-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/settingssetting-idset-post-openapi.md
- name: Foursquare Post Specials Add
  x-api-slug: foursquare
  description: /specials/{SPECIAL_ID}
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///specials/add
  tags: Specials
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/specialsadd-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/specialsadd-post-openapi.md
- name: Foursquare Get Specials List
  x-api-slug: foursquare
  description: /specials/add
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///specials/list
  tags: Specials,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/specialslist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/specialslist-get-openapi.md
- name: Foursquare Get Specials Search
  x-api-slug: foursquare
  description: /specials/list
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///specials/search
  tags: Specials,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/specialssearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/specialssearch-get-openapi.md
- name: Foursquare Post Specials Flag
  x-api-slug: foursquare
  description: /specials/{SPECIAL_ID}/configuration
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///specials/{ID}/flag
  tags: Specials,Flag
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/specialsidflag-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/specialsidflag-post-openapi.md
- name: Foursquare Get Specials
  x-api-slug: foursquare
  description: /settings/{SETTING_ID}/set
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///specials/{SPECIAL_ID}
  tags: Specials
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/specialsspecial-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/specialsspecial-id-get-openapi.md
- name: Foursquare Get Specials Configuration
  x-api-slug: foursquare
  description: /specials/search
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///specials/{SPECIAL_ID}/configuration
  tags: Specials,Configuration
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/specialsspecial-idconfiguration-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/specialsspecial-idconfiguration-get-openapi.md
- name: Foursquare Post Specials Retire
  x-api-slug: foursquare
  description: /specials/{ID}/flag
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///specials/{SPECIAL_ID}/retire
  tags: Specials,Retire
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/specialsspecial-idretire-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/specialsspecial-idretire-post-openapi.md
- name: Foursquare Post Tips Add
  x-api-slug: foursquare
  description: /tips/{TIP_ID}
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///tips/add
  tags: Tips
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/tipsadd-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/tipsadd-post-openapi.md
- name: Foursquare Get Tips Search
  x-api-slug: foursquare
  description: /tips/add
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///tips/search
  tags: Tips,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/tipssearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/tipssearch-get-openapi.md
- name: Foursquare Get Tips
  x-api-slug: foursquare
  description: /checkins/{CHECKIN_ID}/deletecomment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///tips/{TIP_ID}
  tags: Tips
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/tipstip-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/tipstip-id-get-openapi.md
- name: Foursquare Get Tips Done
  x-api-slug: foursquare
  description: /tips/search
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///tips/{TIP_ID}/done
  tags: Tips,Done
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/tipstip-iddone-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/tipstip-iddone-get-openapi.md
- name: Foursquare Get Tips Listed
  x-api-slug: foursquare
  description: /tips/{TIP_ID}/done
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///tips/{TIP_ID}/listed
  tags: Tips,Listed
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/tipstip-idlisted-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/tipstip-idlisted-get-openapi.md
- name: Foursquare Post Tips Markdone
  x-api-slug: foursquare
  description: /tips/{TIP_ID}/listed
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///tips/{TIP_ID}/markdone
  tags: Tips,Markdone
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/tipstip-idmarkdone-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/tipstip-idmarkdone-post-openapi.md
- name: Foursquare Post Tips Marktodo
  x-api-slug: foursquare
  description: /tips/{TIP_ID}/markdone
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///tips/{TIP_ID}/marktodo
  tags: Tips,Marktodo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/tipstip-idmarktodo-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/tipstip-idmarktodo-post-openapi.md
- name: Foursquare Post Tips Unmark
  x-api-slug: foursquare
  description: /tips/{TIP_ID}/marktodo
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///tips/{TIP_ID}/unmark
  tags: Tips,Unmark
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/tipstip-idunmark-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/tipstip-idunmark-post-openapi.md
- name: Foursquare Post Updates Marknotificationsread
  x-api-slug: foursquare
  description: /updates/notifications
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///updates/marknotificationsread
  tags: S,Marknotificationsread
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/updatesmarknotificationsread-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/updatesmarknotificationsread-post-openapi.md
- name: Foursquare Get Updates Notifications
  x-api-slug: foursquare
  description: /updates/{UPDATE_ID}
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///updates/notifications
  tags: S,Notifications
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/updatesnotifications-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/updatesnotifications-get-openapi.md
- name: Foursquare Get Updates Update
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/updateitem
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///updates/{UPDATE_ID}
  tags: S
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/updatesupdate-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/updatesupdate-id-get-openapi.md
- name: Foursquare Get Users Leaderboard
  x-api-slug: foursquare
  description: /users/{USER_ID}
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/leaderboard
  tags: Users,Leaderboard
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersleaderboard-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersleaderboard-get-openapi.md
- name: Foursquare Get Users Requests
  x-api-slug: foursquare
  description: /users/leaderboard
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/requests
  tags: Users,Requests
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersrequests-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersrequests-get-openapi.md
- name: Foursquare Get Users Search
  x-api-slug: foursquare
  description: /users/requests
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/search
  tags: Users,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/userssearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/userssearch-get-openapi.md
- name: Foursquare Post Users Search
  x-api-slug: foursquare
  description: users/search (GET)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/search
  tags: Users,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/userssearch-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/userssearch-post-openapi.md
- name: Foursquare Post Users Self Update
  x-api-slug: foursquare
  description: /users/{USER_ID}/unfriend
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/self/update
  tags: Users,Self
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersselfupdate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersselfupdate-post-openapi.md
- name: Foursquare Get Users
  x-api-slug: foursquare
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-id-get-openapi.md
- name: Foursquare Post Users Approve
  x-api-slug: foursquare
  description: /users/{USER_ID}/venuehistory
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/approve
  tags: Users,Approve
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idapprove-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idapprove-post-openapi.md
- name: Foursquare Get Users Badges
  x-api-slug: foursquare
  description: users/search (POST)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/badges
  tags: Users,Badges
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idbadges-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idbadges-get-openapi.md
- name: Foursquare Get Users Checkins
  x-api-slug: foursquare
  description: /users/{USER_ID}/badges
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/checkins
  tags: Users,Checkins
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idcheckins-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idcheckins-get-openapi.md
- name: Foursquare Post Users Deny
  x-api-slug: foursquare
  description: /users/{USER_ID}/approve
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/deny
  tags: Users,Deny
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-iddeny-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-iddeny-post-openapi.md
- name: Foursquare Get Users Friends
  x-api-slug: foursquare
  description: /users/{USER_ID}/checkins
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/friends
  tags: Users,Friends
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idfriends-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idfriends-get-openapi.md
- name: Foursquare Get Users Lists
  x-api-slug: foursquare
  description: /users/{USER_ID}/friends
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/lists
  tags: Users,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idlists-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idlists-get-openapi.md
- name: Foursquare Get Users Mayorships
  x-api-slug: foursquare
  description: /users/{USER_ID}/lists
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/mayorships
  tags: Users,Mayorships
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idmayorships-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idmayorships-get-openapi.md
- name: Foursquare Get Users Photos
  x-api-slug: foursquare
  description: /users/{USER_ID}/mayorships
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/photos
  tags: Users,Photos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idphotos-get-openapi.md
- name: Foursquare Post Users Request
  x-api-slug: foursquare
  description: /users/{USER_ID}/deny
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/request
  tags: Users,Request
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idrequest-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idrequest-post-openapi.md
- name: Foursquare Post Users Setpings
  x-api-slug: foursquare
  description: /users/{USER_ID}/request
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/setpings
  tags: Users,Setpings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idsetpings-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idsetpings-post-openapi.md
- name: Foursquare Get Users Tips
  x-api-slug: foursquare
  description: /users/{USER_ID}/photos
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/tips
  tags: Users,Tips
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idtips-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idtips-get-openapi.md
- name: Foursquare Get Users Todos
  x-api-slug: foursquare
  description: /users/{USER_ID}/tips
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/todos
  tags: Users,Todos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idtodos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idtodos-get-openapi.md
- name: Foursquare Post Users Unfriend
  x-api-slug: foursquare
  description: /users/{USER_ID}/setpings
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/unfriend
  tags: Users,Unfriend
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idunfriend-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idunfriend-post-openapi.md
- name: Foursquare Get Users Venuehistory
  x-api-slug: foursquare
  description: /users/{USER_ID}/todos
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/venuehistory
  tags: Users,Venuehistory
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idvenuehistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/usersuser-idvenuehistory-get-openapi.md
- name: Foursquare Post Venuegroups Add
  x-api-slug: foursquare
  description: /venuegroups/{GROUP_ID}
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venuegroups/add
  tags: Venuegroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuegroupsadd-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuegroupsadd-post-openapi.md
- name: Foursquare Get Venuegroups List
  x-api-slug: foursquare
  description: /venuegroups/{GROUP_ID}/delete
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venuegroups/list
  tags: Venuegroups,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuegroupslist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuegroupslist-get-openapi.md
- name: Foursquare Get Venuegroups Group
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/proposeedit
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venuegroups/{GROUP_ID}
  tags: Venuegroups,Group
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuegroupsgroup-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuegroupsgroup-id-get-openapi.md
- name: Foursquare Post Venuegroups Group Addvenue
  x-api-slug: foursquare
  description: /venuegroups/list
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venuegroups/{GROUP_ID}/addvenue
  tags: Venuegroups,Group,Venue
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuegroupsgroup-idaddvenue-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuegroupsgroup-idaddvenue-post-openapi.md
- name: Foursquare Post Venuegroups Group Delete
  x-api-slug: foursquare
  description: /venuegroups/add
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venuegroups/{GROUP_ID}/delete
  tags: Venuegroups,Group
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuegroupsgroup-iddelete-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuegroupsgroup-iddelete-post-openapi.md
- name: Foursquare Post Venuegroups Group Removevenue
  x-api-slug: foursquare
  description: /venuegroups/{GROUP_ID}/addvenue
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venuegroups/{GROUP_ID}/removevenue
  tags: Venuegroups,Group,Removevenue
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuegroupsgroup-idremovevenue-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuegroupsgroup-idremovevenue-post-openapi.md
- name: Foursquare Post Venues Add
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/add
  tags: Venues
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesadd-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesadd-post-openapi.md
- name: Foursquare Get Venues Categories
  x-api-slug: foursquare
  description: /venues/add
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/categories
  tags: Venues,Categories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuescategories-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuescategories-get-openapi.md
- name: Foursquare Get Venues Explore
  x-api-slug: foursquare
  description: /venues/categories
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/explore
  tags: Venues,Explore
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesexplore-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesexplore-get-openapi.md
- name: Foursquare Get Venues Managed
  x-api-slug: foursquare
  description: /venues/explore
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/managed
  tags: Venues,Managed
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesmanaged-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesmanaged-get-openapi.md
- name: Foursquare Get Venues Search
  x-api-slug: foursquare
  description: /venues/managed
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/search
  tags: Venues,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuessearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuessearch-get-openapi.md
- name: Foursquare Get Venues Suggestcompletion
  x-api-slug: foursquare
  description: /venues/search
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/suggestcompletion
  tags: Venues,Suggestcompletion
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuessuggestcompletion-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuessuggestcompletion-get-openapi.md
- name: Foursquare Get Venues Timeseries
  x-api-slug: foursquare
  description: /venues/suggestcompletion
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/timeseries
  tags: Venues,Timeseries
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuestimeseries-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuestimeseries-get-openapi.md
- name: Foursquare Get Venues Trending
  x-api-slug: foursquare
  description: /venues/timeseries
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/trending
  tags: Venues,Trending
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuestrending-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuestrending-get-openapi.md
- name: Foursquare Get Venues
  x-api-slug: foursquare
  description: /users/self/update
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}
  tags: Venues
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-id-get-openapi.md
- name: Foursquare Post Venues Edit
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/tips
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/edit
  tags: Venues,Edit
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idedit-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idedit-post-openapi.md
- name: Foursquare Get Venues Events
  x-api-slug: foursquare
  description: /venues/trending
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/events
  tags: Venues,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idevents-get-openapi.md
- name: Foursquare Post Venues Flag
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/edit
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/flag
  tags: Venues,Flag
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idflag-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idflag-post-openapi.md
- name: Foursquare Get Venues Herenow
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/events
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/herenow
  tags: Venues,Herenow
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idherenow-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idherenow-get-openapi.md
- name: Foursquare Get Venues Links
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/herenow
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/links
  tags: Venues,Links
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idlinks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idlinks-get-openapi.md
- name: Foursquare Get Venues Listed
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/links
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/listed
  tags: Venues,Listed
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idlisted-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idlisted-get-openapi.md
- name: Foursquare Post Venues Marktodo
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/flag
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/marktodo
  tags: Venues,Marktodo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idmarktodo-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idmarktodo-post-openapi.md
- name: Foursquare Get Venues Menu
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/listed
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/menu
  tags: Venues,Menu
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idmenu-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idmenu-get-openapi.md
- name: Foursquare Get Venues Photos
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/menu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/photos
  tags: Venues,Photos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idphotos-get-openapi.md
- name: Foursquare Post Venues Proposeedit
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/marktodo
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/proposeedit
  tags: Venues,Proposeedit
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idproposeedit-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idproposeedit-post-openapi.md
- name: Foursquare Get Venues Similar
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/photos
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/similar
  tags: Venues,Similar
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idsimilar-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idsimilar-get-openapi.md
- name: Foursquare Get Venues Stats
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/similar
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/stats
  tags: Venues,Stats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idstats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idstats-get-openapi.md
- name: Foursquare Get Venues Tips
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/stats
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/tips
  tags: Venues,Tips
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idtips-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/venuesvenue-idtips-get-openapi.md
- name: Foursquare
  x-api-slug: foursquare
  description: foursquare makes the real world easier to use. We build tools that
    help you keep up with friends, discover whats nearby, save money and unlock deals.
    Whether youre setting off on a trip around the world, coordinating a night out
    with friends, or trying to pick out the best dish at your local restaurant, foursquare
    is the perfect companion. The foursquare API gives you access to all of the data
    used by the foursquare mobile applications, and, in some cases, even more.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2/
  tags: Foursquare
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/foursquare/master/_listings/foursquare/openapi.md
x-common:
- type: x-api-json--authoritative
  url: http://apis.io/apisdef/legacy/foursquare.json
- type: x-apigee-console
  url: https://api.apigee.com/v1/consoles/foursquare/apidescription?format=internal&ver=1393644831000
- type: x-application-management
  url: https://foursquare.com/developers/apps
- type: x-blog
  url: http://engineering.foursquare.com/
- type: x-blog-rss
  url: http://engineering.foursquare.com/feed/
- type: x-curated-source
  url: http://blog.foursquare.com/2013/09/17/we-put-a-fresh-coat-of-paint-on-foursquare-for-ios-7/
- type: x-website
  url: http://blog.foursquare.com
- type: x-crunchbase
  url: http://www.crunchbase.com/company/foursquare
- type: x-crunchbase
  url: https://crunchbase.com/organization/foursquare
- type: x-email
  url: support@foursquare.com
- type: x-email
  url: ads@foursquare.com
- type: x-email
  url: press@foursquare.com
- type: x-email
  url: security@foursquare.com
- type: x-email
  url: feedback@foursquare.com
- type: x-email
  url: privacy@foursquare.com
- type: x-error-codes
  url: https://developer.foursquare.com/overview/responses
- type: x-foursquare
  url: http://foursquare.com/nasa
- type: x-foursquare
  url: http://foursquare.com/yourcommissary
- type: x-getting-started
  url: https://developer.foursquare.com/start
- type: x-github
  url: https://github.com/foursquare
- type: x-privacy
  url: https://foursquare.com/legal/privacy
- type: x-rate-limits
  url: https://developer.foursquare.com/overview/ratelimits
- type: x-stack-overflow
  url: http://stackoverflow.com/questions/tagged/foursquare
- type: x-terms-of-service
  url: https://developer.foursquare.com/overview/community
- type: x-twitter
  url: https://twitter.com/foursquare
- type: x-twitter
  url: https://twitter.com/foursquareapi
- type: x-website
  url: http://foursquare.com
- type: x-website
  url: https://developer.foursquare.com/
- type: x-website
  url: https://foursquare.com/apps/slack
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---