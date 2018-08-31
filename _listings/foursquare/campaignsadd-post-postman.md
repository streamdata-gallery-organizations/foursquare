{
  "info": {
    "name": "Foursquare Post Campaigns Add",
    "_postman_id": "f3e5929a-7c86-4aa0-a54a-e74713ed6b48",
    "description": "/campaigns/{CAMPAIGN_ID}",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Campaigns",
      "item": [
        {
          "id": "829a2526-dbcc-4077-ba56-505f72d4b2e9",
          "name": "campaignscampaign-id",
          "request": {
            "url": "http://api.foursquare.com/v2/campaigns/add?campaignId=%7B%7D&endAt=%7B%7D&groupId=%7B%7D&specialId=%7B%7D&startAt=%7B%7D&v=%7B%7D&venueId=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/{CAMPAIGN_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd74f6b8-d6e5-46d3-94cf-48286ae3109e"
            }
          ]
        }
      ]
    }
  ]
}