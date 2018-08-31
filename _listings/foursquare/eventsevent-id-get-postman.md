{
  "info": {
    "name": "Foursquare Get Events Event",
    "_postman_id": "2ecbba06-5ec1-4458-8c2d-9e1b76c672b0",
    "description": "/campaigns/{CAMPAIGN_ID}/start",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Events",
      "item": [
        {
          "id": "9398f919-daad-4d08-8547-f45ea0d81ed6",
          "name": "eventsevent-id",
          "request": {
            "url": "http://api.foursquare.com/v2/events/categories?v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/events/{EVENT_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0cd9660d-0b47-455a-b6d3-73f433137e8a"
            }
          ]
        },
        {
          "id": "8136ed24-f80a-4673-b43d-d6d0d8563308",
          "name": "eventscategories",
          "request": {
            "url": "http://api.foursquare.com/v2/events/search?domain=%7B%7D&eventId=%7B%7D&participantId=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/events/categories"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c45b5b34-326e-4126-99a5-7f828d3cc403"
            }
          ]
        },
        {
          "id": "c7a2190d-e366-4093-9377-67a28019a056",
          "name": "campaignscampaign-idstart",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "events/:EVENT_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "EVENT_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/{CAMPAIGN_ID}/start"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e10c92d4-84a1-4a09-a437-44cc832ecfed"
            }
          ]
        }
      ]
    }
  ]
}