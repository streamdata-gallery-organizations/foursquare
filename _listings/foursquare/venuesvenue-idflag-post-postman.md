{
  "info": {
    "name": "Foursquare Post Venues Flag",
    "_postman_id": "63d4fbe1-1239-439a-a700-676f1a282b30",
    "description": "/venues/{VENUE_ID}/edit",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Campaigns",
      "item": [
        {
          "id": "540a53e4-2b2a-41d3-9488-c5b3e93bed8c",
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
              "id": "5ca1fc00-73bc-452c-989a-a10006e55c14"
            }
          ]
        },
        {
          "id": "b9ef9384-41e3-47e3-96b7-c70e5080d1d4",
          "name": "campaignsadd",
          "request": {
            "url": "http://api.foursquare.com/v2/campaigns/list?groupId=%7B%7D&specialId=%7B%7D&status=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "265d5936-7482-4dd8-abcc-de7c5f898d91"
            }
          ]
        },
        {
          "id": "e0af134f-f385-411a-a047-8a4360cfc991",
          "name": "specialsspecial-idretire",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "campaigns/:CAMPAIGN_ID"
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
                  "id": "CAMPAIGN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/{SPECIAL_ID}/retire"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e300906-6776-4aab-826d-7a9f708d2321"
            }
          ]
        },
        {
          "id": "82b9160b-07c5-499f-b7fb-61a182c7a711",
          "name": "campaignscampaign-idtimeseries",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "campaigns/:CAMPAIGN_ID/delete"
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
                  "id": "CAMPAIGN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/{CAMPAIGN_ID}/timeseries"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c9b2a7e7-9144-496a-9dfa-c2bbfa31b2ed"
            }
          ]
        },
        {
          "id": "63683fcf-831f-46df-a015-d358293b6b00",
          "name": "campaignscampaign-iddelete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "campaigns/:CAMPAIGN_ID/end"
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
                  "id": "CAMPAIGN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/{CAMPAIGN_ID}/delete"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4ae1df6-900c-4657-9c04-c7868740a1ba"
            }
          ]
        },
        {
          "id": "97ff5f8c-2c08-4f16-a651-da44ada021db",
          "name": "campaignscampaign-idend",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "campaigns/:CAMPAIGN_ID/start"
              ],
              "query": [
                {
                  "key": "startAt",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CAMPAIGN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/{CAMPAIGN_ID}/end"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89578e4c-9568-481c-a085-f7bf0f05c150"
            }
          ]
        },
        {
          "id": "0ef13fcc-7f98-438a-8e52-7b54feb2857d",
          "name": "campaignslist",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "campaigns/:CAMPAIGN_ID/timeseries"
              ],
              "query": [
                {
                  "key": "endAt",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startAt",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CAMPAIGN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "124bef2d-d789-4c38-b8e2-6de5761b5efe"
            }
          ]
        }
      ]
    },
    {
      "name": "Checkins",
      "item": [
        {
          "id": "61484f4b-989c-46a0-9c42-5cc9d4e50577",
          "name": "checkinscheckin-id",
          "request": {
            "url": "http://api.foursquare.com/v2/checkins/add?alt=%7B%7D&altAcc=%7B%7D&broadcast=%7B%7D&eventId=%7B%7D&ll=%7B%7D&llAcc=%7B%7D&shout=%7B%7D&v=%7B%7D&venue=%7B%7D&venueId=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/checkins/{CHECKIN_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c71518af-b2f3-436e-949c-3c8032e7f426"
            }
          ]
        },
        {
          "id": "a0dc4458-f21f-4169-8e2b-ed8c07aa54c5",
          "name": "checkinsadd",
          "request": {
            "url": "http://api.foursquare.com/v2/checkins/recent?afterTimestamp=%7B%7D&limit=%7B%7D&ll=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/checkins/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "348c6349-e24b-4883-b2a6-0861c91d4c4c"
            }
          ]
        },
        {
          "id": "251b6b56-4c1a-4612-b195-304a920ecf4f",
          "name": "venuegroupsgroup-idremovevenue",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "checkins/:CHECKIN_ID"
              ],
              "query": [
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CHECKIN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/venuegroups/{GROUP_ID}/removevenue"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce39a69d-1940-455a-b42f-a44285136040"
            }
          ]
        },
        {
          "id": "fb9b7152-8281-4351-8bcf-3916f2588ed1",
          "name": "checkinsrecent",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "checkins/:CHECKIN_ID/addcomment"
              ],
              "query": [
                {
                  "key": "text",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CHECKIN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/checkins/recent"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0d875bc9-d328-4fa3-9ef6-594533b60df0"
            }
          ]
        },
        {
          "id": "0a3e4678-9941-4338-a89a-3fccf1d22bea",
          "name": "checkinscheckin-idaddcomment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "checkins/:CHECKIN_ID/deletecomment"
              ],
              "query": [
                {
                  "key": "commentId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CHECKIN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/checkins/{CHECKIN_ID}/addcomment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f9d900e-c736-4cda-a1be-d20ebe90da08"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "87b06f91-6581-40f6-8538-24990216c7cb",
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
              "id": "ebc8972b-4ff0-4d47-b890-fd699e8ce86c"
            }
          ]
        },
        {
          "id": "52a3b800-1419-4f1b-9b33-35b6e5afcca0",
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
              "id": "97dc8d3d-2d72-4b69-bca9-bfbd1d897cef"
            }
          ]
        },
        {
          "id": "7b2ccae7-082e-4320-af7e-eac077fd5fcd",
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
              "id": "a8967b18-6e80-491f-9eb0-16ab4b6434cb"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "61010239-58d4-4285-b1ea-78b20157f77c",
          "name": "listslist-id",
          "request": {
            "url": "http://api.foursquare.com/v2/lists/add?collaborative=%7B%7D&description=%7B%7D&name=%7B%7D&photoId=%7B%7D&v=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b53cb248-4d33-4c68-b9ab-7efe9a2c4d98"
            }
          ]
        },
        {
          "id": "2857eb9a-ad9f-4923-9c21-b89c0d590dc3",
          "name": "tipstip-idunmark",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/{TIP_ID}/unmark"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a8aadd7-35f4-4f6d-b45b-07ec814695dd"
            }
          ]
        },
        {
          "id": "b042834a-4b82-4ef9-a4fe-af79d0316d42",
          "name": "listslist-idsuggestvenues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/additem"
              ],
              "query": [
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "listId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "text",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tipId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "url",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venueId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/suggestvenues"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85f6e152-7b95-44a2-a553-3aba0c01cc00"
            }
          ]
        },
        {
          "id": "f839d3b4-9e1a-4362-b78c-689e15e101c1",
          "name": "listslist-idadditem",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/deleteitem"
              ],
              "query": [
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/additem"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92565a4b-5b29-4937-9f95-15987bcf0ba1"
            }
          ]
        },
        {
          "id": "1e73f5c1-e0c3-4dc1-a84c-c13f96477373",
          "name": "listslist-iddeleteitem",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/follow"
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
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/deleteitem"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "092f8cd6-84c5-49c6-86f3-2ad1fb39f1c9"
            }
          ]
        },
        {
          "id": "72d61a97-a830-4777-80e2-2f0c50489eef",
          "name": "listsadd",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/followers"
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
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "983e3a6e-e163-44e7-bc40-2578215d2efb"
            }
          ]
        },
        {
          "id": "0ea7e668-a30b-4485-bfc1-4afa040fc799",
          "name": "listslist-idfollow",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/moveitem"
              ],
              "query": [
                {
                  "key": "afterId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "beforeId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/follow"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa9f6869-29ea-4995-893b-3672a158bc33"
            }
          ]
        },
        {
          "id": "3ce575a9-00bc-4f80-88de-2f1d9eefaa60",
          "name": "listslist-idmoveitem",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/share"
              ],
              "query": [
                {
                  "key": "broadcast",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/moveitem"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36a24fd1-1e7b-4190-b130-e4de72e34207"
            }
          ]
        },
        {
          "id": "31fd797c-43af-4a87-9394-ab85cec8de5c",
          "name": "listslist-idfollowers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/suggestphoto"
              ],
              "query": [
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/followers"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "275c6066-a2eb-45a1-ad9c-ac7971a72eac"
            }
          ]
        },
        {
          "id": "a2313290-8208-40fe-93a6-58cf2592acce",
          "name": "listslist-idsuggestphoto",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/suggesttip"
              ],
              "query": [
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/suggestphoto"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6571c607-8c56-48d4-868a-ee35ea40a475"
            }
          ]
        },
        {
          "id": "54fb695c-6f91-4d74-a442-36dfa8c8b0a9",
          "name": "listslist-idsuggesttip",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/suggestvenues"
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
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/suggesttip"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88453a86-e4ed-4969-a391-c2b404b891fc"
            }
          ]
        },
        {
          "id": "e5b0c3d5-170e-4e65-8b39-dab86b5ea0d0",
          "name": "listslist-idshare",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/unfollow"
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
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/share"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a125c331-9ad8-41ec-a119-2aa09b3fad27"
            }
          ]
        },
        {
          "id": "5182e859-cc21-42fe-9059-a2f57ab7e965",
          "name": "listslist-idunfollow",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/update"
              ],
              "query": [
                {
                  "key": "collaborative",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "photoId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/unfollow"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55768d88-c29f-4d55-ab28-125b076c6a31"
            }
          ]
        },
        {
          "id": "87830566-2826-44a4-ad78-e20a683c323a",
          "name": "listslist-idupdate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/updateitem"
              ],
              "query": [
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "photoId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "text",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tipId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "url",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/update"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fcfbc578-fcdd-4428-b6e0-57bb0dd72749"
            }
          ]
        }
      ]
    },
    {
      "name": "Multi",
      "item": [
        {
          "id": "2b0ebef4-2cfe-4ff3-b8e1-bfd2b13f4d5d",
          "name": "pagespage-idvenues",
          "request": {
            "url": "http://api.foursquare.com/v2/multi?requests=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/pages/{PAGE_ID}/venues"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99b4d33b-c940-442c-ab5b-4bd710d28445"
            }
          ]
        }
      ]
    },
    {
      "name": "Pages",
      "item": [
        {
          "id": "f108960a-08e0-4888-98a9-fd5097116e68",
          "name": "pagespage-id",
          "request": {
            "url": "http://api.foursquare.com/v2/pages/search?fbid=%7B%7D&name=%7B%7D&twitter=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/pages/{PAGE_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e909bc0-889b-427e-9a15-cfa8e7c12338"
            }
          ]
        },
        {
          "id": "7e397322-6e8b-4cab-8426-967fc2bb95fd",
          "name": "eventssearch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "pages/:PAGE_ID"
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
                  "id": "PAGE_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/events/search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb071474-d0fa-47ce-ac8b-8cffea945e31"
            }
          ]
        },
        {
          "id": "e7e2a605-7ffe-41c7-aacf-3bb14179bc72",
          "name": "pagessearch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "pages/:PAGE_ID/venues"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ll",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ne",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "radius",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sw",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "PAGE_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/pages/search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0d576be-1a82-42b4-805a-b2cc29edafed"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "d9f8e4e4-aaea-4c7c-b93f-e58c7c851803",
          "name": "photosphoto-id",
          "request": {
            "url": "http://api.foursquare.com/v2/photos/add?alt=%7B%7D&altAcc=%7B%7D&broadcast=%7B%7D&checkinId=%7B%7D&Content-Type=%7B%7D&image=%7B%7D&ll=%7B%7D&llAcc=%7B%7D&public=%7B%7D&tipId=%7B%7D&v=%7B%7D&venueId=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/photos/{PHOTO_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e95cb99-4c16-463b-a54c-d0078fab34be"
            }
          ]
        },
        {
          "id": "fdfe194e-74c1-4c27-a1d4-61abcfcf33c2",
          "name": "updatesmarknotificationsread",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "photos/:PHOTO_ID"
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
                  "id": "PHOTO_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/updates/marknotificationsread"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f2e8668-e076-49ee-9314-f8f2f89f6750"
            }
          ]
        }
      ]
    },
    {
      "name": "Settings",
      "item": [
        {
          "id": "38fcb5bc-e935-495a-aa8e-7cfd3384daa3",
          "name": "settingssetting-id",
          "request": {
            "url": "http://api.foursquare.com/v2/settings/all?v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/settings/{SETTING_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43ac79b5-e10f-421a-91bd-387bd6ac5de4"
            }
          ]
        },
        {
          "id": "1e6c8dc6-42f8-4253-90aa-1848fa4a2e0f",
          "name": "photosadd",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "settings/:SETTING_ID"
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
                  "id": "SETTING_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/photos/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "636e18f9-ff2b-47a1-859e-1fe628088d68"
            }
          ]
        },
        {
          "id": "b8e49fae-8b48-4198-8802-87435c47b672",
          "name": "settingsall",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "settings/:SETTING_ID/set"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "value",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "SETTING_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/settings/all"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93c98817-531e-4406-8edd-ef62bbe02130"
            }
          ]
        }
      ]
    },
    {
      "name": "Specials",
      "item": [
        {
          "id": "1e778854-0088-4be8-b9e4-d3dc6c9a18f5",
          "name": "specialsspecial-id",
          "request": {
            "url": "http://api.foursquare.com/v2/specials/add?cost=%7B%7D&count1=%7B%7D&count2=%7B%7D&count3=%7B%7D&finePrint=%7B%7D&name=%7B%7D&offerId=%7B%7D&text=%7B%7D&type=%7B%7D&unlockedText=%7B%7D&v=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/{SPECIAL_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "389b62fa-d46b-42a8-9699-165d93da245e"
            }
          ]
        },
        {
          "id": "bd53f79b-0a9d-40eb-909c-d3eb522552e9",
          "name": "specialsadd",
          "request": {
            "url": "http://api.foursquare.com/v2/specials/list?status=%7B%7D&v=%7B%7D&venueId=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1b50890-49cd-48f6-b8a1-24c8d6f16512"
            }
          ]
        },
        {
          "id": "297d5c78-48f6-44b3-94f4-10968b5c1806",
          "name": "specialslist",
          "request": {
            "url": "http://api.foursquare.com/v2/specials/search?alt=%7B%7D&altAcc=%7B%7D&limit=%7B%7D&ll=%7B%7D&llAcc=%7B%7D&radius=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "139ba0a7-2c97-4a30-a735-b6e45fbaf5cb"
            }
          ]
        },
        {
          "id": "9afd86fb-d3bf-4584-b556-0a6e1b0dd3bc",
          "name": "specialsspecial-idconfiguration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "specials/:ID/flag"
              ],
              "query": [
                {
                  "key": "problem",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "text",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venueId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/{SPECIAL_ID}/configuration"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e47771f-66f0-4bb7-a54f-000f5f55e089"
            }
          ]
        },
        {
          "id": "a2fe54e0-de66-4a11-b355-e3d1a4f83b32",
          "name": "settingssetting-idset",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "specials/:SPECIAL_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venueId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "SPECIAL_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/settings/{SETTING_ID}/set"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7df28909-75ee-418d-88fb-0d9add2eb327"
            }
          ]
        },
        {
          "id": "a7cca534-6988-48d0-83a9-05288f4489ce",
          "name": "specialssearch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "specials/:SPECIAL_ID/configuration"
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
                  "id": "SPECIAL_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5855c6bf-3df2-4f33-ba31-d03923783ccc"
            }
          ]
        },
        {
          "id": "3e7e8d72-c2e5-4c84-8760-9c08429085d2",
          "name": "specialsidflag",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "specials/:SPECIAL_ID/retire"
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
                  "id": "SPECIAL_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/{ID}/flag"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "afc7ffa3-34e8-42b6-bfa3-10c9f4f1f682"
            }
          ]
        }
      ]
    },
    {
      "name": "Tips",
      "item": [
        {
          "id": "c35e86f9-bea2-435c-88ea-9a71f2e30cb0",
          "name": "tipstip-id",
          "request": {
            "url": "http://api.foursquare.com/v2/tips/add?broadcast=%7B%7D&text=%7B%7D&url=%7B%7D&v=%7B%7D&venueId=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/{TIP_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a34f482-6154-4e3f-808f-6303df123a0a"
            }
          ]
        },
        {
          "id": "37b78fc3-15b0-4292-aa44-afe025f764a2",
          "name": "tipsadd",
          "request": {
            "url": "http://api.foursquare.com/v2/tips/search?filter=%7B%7D&limit=%7B%7D&ll=%7B%7D&offset=%7B%7D&query=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1bc106f0-6db3-4222-a6ea-9d58c88b98d3"
            }
          ]
        },
        {
          "id": "2cc6ad5a-bc0b-4bf1-8b8f-39ea29795098",
          "name": "checkinscheckin-iddeletecomment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "tips/:TIP_ID"
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
                  "id": "TIP_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/checkins/{CHECKIN_ID}/deletecomment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3eb25106-0c6b-40a0-8245-be864d09ff18"
            }
          ]
        },
        {
          "id": "c4617134-cfa9-4c5f-a6a7-352c4e1c0b8a",
          "name": "tipssearch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "tips/:TIP_ID/done"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "TIP_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4d61464-ae3b-4742-9ba5-1f7f010e2ffd"
            }
          ]
        },
        {
          "id": "8a0681b2-cd91-47bf-8cfa-e78aade23f72",
          "name": "tipstip-iddone",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "tips/:TIP_ID/listed"
              ],
              "query": [
                {
                  "key": "group",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "TIP_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/{TIP_ID}/done"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8b90ef7-c26c-45fe-b571-e8c1f7a69dad"
            }
          ]
        },
        {
          "id": "9fa1ea66-df4a-406c-8a27-9f87f37406c9",
          "name": "tipstip-idlisted",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "tips/:TIP_ID/markdone"
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
                  "id": "TIP_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/{TIP_ID}/listed"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "97bb3994-2ebf-462e-b0c0-0302db02b5f1"
            }
          ]
        },
        {
          "id": "b6925845-380e-45ee-a364-754346d2e41a",
          "name": "tipstip-idmarkdone",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "tips/:TIP_ID/marktodo"
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
                  "id": "TIP_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/{TIP_ID}/markdone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b807cc94-565a-4c4c-8e2f-9128fab3daaa"
            }
          ]
        },
        {
          "id": "a1def2e0-995b-42c6-b819-e04bb7ad25b2",
          "name": "tipstip-idmarktodo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "tips/:TIP_ID/unmark"
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
                  "id": "TIP_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/{TIP_ID}/marktodo"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9db399dd-3269-4674-be47-cc7912e72d33"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "038d3a03-d245-4b0c-abda-5e8a7520b3e2",
          "name": "updatesnotifications",
          "request": {
            "url": "http://api.foursquare.com/v2/updates/marknotificationsread?highWatermark=%7B%7D&v=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/updates/notifications"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b23d2c25-2278-4ba0-bb55-42b2c2b35f44"
            }
          ]
        },
        {
          "id": "71fcc893-603f-4e2b-87d9-f8ac1fbf4773",
          "name": "updatesupdate-id",
          "request": {
            "url": "http://api.foursquare.com/v2/updates/notifications?limit=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/updates/{UPDATE_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3a723af-0011-4a43-ac28-52a697efe4d1"
            }
          ]
        },
        {
          "id": "c329d145-8a7e-4622-b998-8c56bed81986",
          "name": "listslist-idupdateitem",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "updates/:UPDATE_ID"
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
                  "id": "UPDATE_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/updateitem"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "18c20516-006c-4b7e-b2ed-54eb863be5cd"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "2774a5e8-a1d9-4abc-b183-0210138d30fc",
          "name": "usersuser-id",
          "request": {
            "url": "http://api.foursquare.com/v2/users/leaderboard?neighbors=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/users/{USER_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe98e59e-42fc-42eb-b4db-c0723a001c72"
            }
          ]
        },
        {
          "id": "7cbdf4d5-f99f-4af1-84e2-69bd82941f70",
          "name": "usersleaderboard",
          "request": {
            "url": "http://api.foursquare.com/v2/users/requests?v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/users/leaderboard"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe3cdc5f-af58-4ff0-9e9a-4e2755fcc6c6"
            }
          ]
        },
        {
          "id": "4d19c632-9829-4631-9d2c-2719b8b9c402",
          "name": "usersrequests",
          "request": {
            "url": "http://api.foursquare.com/v2/users/search?email=%7B%7D&fbid=%7B%7D&name=%7B%7D&phone=%7B%7D&twitter=%7B%7D&twitterSource=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/users/requests"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20e69765-5838-44d1-a58b-38e39374db5e"
            }
          ]
        },
        {
          "id": "7283d452-f4df-45c9-a880-6052dc854ac9",
          "name": "userssearch-get",
          "request": {
            "url": "http://api.foursquare.com/v2/users/search?email=%7B%7D&fbid=%7B%7D&name=%7B%7D&phone=%7B%7D&twitter=%7B%7D&twitterSource=%7B%7D&v=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "users/search (GET)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "479d4f1f-0d33-40a1-bf9b-5df44e810f26"
            }
          ]
        },
        {
          "id": "77a874a1-880d-403f-8e60-612e3dff53a2",
          "name": "usersuser-idunfriend",
          "request": {
            "url": "http://api.foursquare.com/v2/users/self/update?Content-Type=%7B%7D&photo=%7B%7D&v=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/users/{USER_ID}/unfriend"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc93fe79-44d6-407e-8eca-006b2a4b3360"
            }
          ]
        },
        {
          "id": "990160b4-c4f7-4206-82c4-3d26858569f4",
          "name": "Get Users",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "users/:USER_ID"
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
                  "id": "USER_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Users"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d527dbc3-4225-40f0-917b-815411de20e6"
            }
          ]
        },
        {
          "id": "db261557-774c-42c7-b43f-3260442f6e13",
          "name": "usersuser-idvenuehistory",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "users/:USER_ID/approve"
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
                  "id": "USER_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/users/{USER_ID}/venuehistory"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd683337-e672-472b-a055-e9fed754f6ed"
            }
          ]
        },
        {
          "id": "6baf2987-2b21-46a8-b10b-5151a1bdf953",
          "name": "userssearch-post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "users/:USER_ID/badges"
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
                  "id": "USER_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "users/search (POST)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac5e4e38-0b7e-4943-a608-786518c6c117"
            }
          ]
        },
        {
          "id": "f6406828-d49e-441a-9c18-113adb850331",
          "name": "usersuser-idbadges",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "users/:USER_ID/checkins"
              ],
              "query": [
                {
                  "key": "afterTimestamp",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "beforeTimestamp",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "USER_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/users/{USER_ID}/badges"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e366f560-c712-4220-a9b1-6e50b9bbc7ac"
            }
          ]
        },
        {
          "id": "de76be2b-54fe-444c-b1ba-9b9117595d51",
          "name": "usersuser-idapprove",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "users/:USER_ID/deny"
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
                  "id": "USER_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/users/{USER_ID}/approve"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "547259f0-ea97-470e-8171-5501d82ade82"
            }
          ]
        },
        {
          "id": "b97e7adf-d02d-42e6-b357-f1e6bb2e5a34",
          "name": "usersuser-idcheckins",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "users/:USER_ID/friends"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "USER_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/users/{USER_ID}/checkins"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5af8c474-622b-45bd-9fc2-baf2db2002c5"
            }
          ]
        },
        {
          "id": "d01c71ec-2b60-44fb-afcd-7b2c92d40f19",
          "name": "usersuser-idfriends",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "users/:USER_ID/lists"
              ],
              "query": [
                {
                  "key": "group",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ll",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "USER_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/users/{USER_ID}/friends"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5014f25-a589-42e2-837a-29c04a39fc12"
            }
          ]
        },
        {
          "id": "0d23e9b5-498a-40b2-a59f-b7b8877e5165",
          "name": "usersuser-idlists",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "users/:USER_ID/mayorships"
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
                  "id": "USER_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/users/{USER_ID}/lists"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "32cbc994-aa92-4bec-9a52-e9839ea9565d"
            }
          ]
        },
        {
          "id": "8569d247-24a3-446a-9d1e-0267ab3b09b9",
          "name": "usersuser-idmayorships",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "users/:USER_ID/photos"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "USER_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/users/{USER_ID}/mayorships"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf00f5d0-c6a7-48e8-8af9-2c390c2602ba"
            }
          ]
        },
        {
          "id": "b161d4c5-f659-442e-bb59-7b6a45b26d5b",
          "name": "usersuser-iddeny",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "users/:USER_ID/request"
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
                  "id": "USER_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/users/{USER_ID}/deny"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "113adcd7-2242-41e5-9c10-acab9b3bf190"
            }
          ]
        },
        {
          "id": "53d4dfe0-3efb-4413-8104-bb8105696a74",
          "name": "usersuser-idrequest",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "users/:USER_ID/setpings"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "value",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "USER_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/users/{USER_ID}/request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "962ac49b-d5a3-4e50-a59a-fffd8f01a3c3"
            }
          ]
        },
        {
          "id": "aecdad5f-396d-4330-a272-e96f36694103",
          "name": "usersuser-idphotos",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "users/:USER_ID/tips"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ll",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "USER_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/users/{USER_ID}/photos"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b61c420-0b56-4800-ba17-87a5f20afbd6"
            }
          ]
        },
        {
          "id": "89aeac26-3e6f-4116-a065-712b456206c4",
          "name": "usersuser-idtips",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "users/:USER_ID/todos"
              ],
              "query": [
                {
                  "key": "ll",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "USER_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/users/{USER_ID}/tips"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "98bc00f8-f0a8-461c-aafa-6345153930e8"
            }
          ]
        },
        {
          "id": "34e96d14-3e7f-4e59-a406-213fa9dc97d9",
          "name": "usersuser-idsetpings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "users/:USER_ID/unfriend"
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
                  "id": "USER_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/users/{USER_ID}/setpings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7760fe4f-3deb-49e3-80f5-37a8df89e65b"
            }
          ]
        },
        {
          "id": "e1d96321-565d-4f57-a1e0-8a16385c503c",
          "name": "usersuser-idtodos",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "users/:USER_ID/venuehistory"
              ],
              "query": [
                {
                  "key": "afterTimestamp",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "beforeTimestamp",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "categoryId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "USER_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/users/{USER_ID}/todos"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08435f33-c3ee-41ce-b449-3ab8bdedc61a"
            }
          ]
        }
      ]
    },
    {
      "name": "Venuegroups",
      "item": [
        {
          "id": "20cfd7ec-fef1-47cf-a2d2-b3a0d65d14d9",
          "name": "venuegroupsgroup-id",
          "request": {
            "url": "http://api.foursquare.com/v2/venuegroups/add?name=%7B%7D&v=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/venuegroups/{GROUP_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3aba0b13-d061-451a-b1aa-60f002055578"
            }
          ]
        },
        {
          "id": "2dfa4766-f076-443f-b7ac-f5828fba536f",
          "name": "venuegroupsgroup-iddelete",
          "request": {
            "url": "http://api.foursquare.com/v2/venuegroups/list?v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/venuegroups/{GROUP_ID}/delete"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1772859-a575-40eb-adda-51cf70cbefb5"
            }
          ]
        },
        {
          "id": "df448835-b945-4269-86ea-3c0c72b80e0b",
          "name": "venuesvenue-idproposeedit",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "venuegroups/:GROUP_ID"
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
                  "id": "GROUP_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/venues/{VENUE_ID}/proposeedit"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "650bdc79-d9bf-47d9-9e4f-d54117c85733"
            }
          ]
        },
        {
          "id": "768adc71-da5b-490f-9994-6e6fd0c263ce",
          "name": "venuegroupslist",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "venuegroups/:GROUP_ID/addvenue"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venueId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "GROUP_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/venuegroups/list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75763738-81eb-463d-96d2-e3e143289a05"
            }
          ]
        },
        {
          "id": "76802795-93e2-4785-8326-1a719c8f36b3",
          "name": "venuegroupsadd",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "venuegroups/:GROUP_ID/delete"
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
                  "id": "GROUP_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/venuegroups/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb90fae8-451b-4772-8d4e-8a46fc9a42fb"
            }
          ]
        },
        {
          "id": "0e64128d-6825-455d-959c-c37a37588726",
          "name": "venuegroupsgroup-idaddvenue",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "venuegroups/:GROUP_ID/removevenue"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venueId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "GROUP_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/venuegroups/{GROUP_ID}/addvenue"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "049d44be-ede2-4b20-9817-4fa82d81dba2"
            }
          ]
        }
      ]
    },
    {
      "name": "Venues",
      "item": [
        {
          "id": "2ea4926a-5457-4ebf-b758-9da410594a9d",
          "name": "venuesvenue-id",
          "request": {
            "url": "http://api.foursquare.com/v2/venues/add?address=%7B%7D&city=%7B%7D&crossStreet=%7B%7D&description=%7B%7D&ignoreDuplicates=%7B%7D&ignoreDuplicatesKey=%7B%7D&ll=%7B%7D&name=%7B%7D&phone=%7B%7D&primaryCategoryId=%7B%7D&state=%7B%7D&twitter=%7B%7D&url=%7B%7D&v=%7B%7D&zip=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/venues/{VENUE_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7339b842-dada-4bf2-98d8-ed7c7d727c6d"
            }
          ]
        },
        {
          "id": "5d2913d2-ca0f-4fa9-bca0-4123754f2f7f",
          "name": "venuesadd",
          "request": {
            "url": "http://api.foursquare.com/v2/venues/categories?v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/venues/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "521d4906-a088-4ed4-abdf-c74111122db7"
            }
          ]
        },
        {
          "id": "3d0ffb51-2547-46af-b411-972505098b1b",
          "name": "venuescategories",
          "request": {
            "url": "http://api.foursquare.com/v2/venues/explore?alt=%7B%7D&altAcc=%7B%7D&intent=%7B%7D&limit=%7B%7D&ll=%7B%7D&llAcc=%7B%7D&novelty=%7B%7D&query=%7B%7D&radius=%7B%7D&section=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/venues/categories"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c51b56c-d803-417a-82d1-1154d81a73a5"
            }
          ]
        },
        {
          "id": "78f81985-cdf8-4c9c-ab79-99e3e02061da",
          "name": "venuesexplore",
          "request": {
            "url": "http://api.foursquare.com/v2/venues/managed?v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/venues/explore"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b5a626a-6041-4bda-820a-0ea93cf6bd85"
            }
          ]
        },
        {
          "id": "417b2c08-51c1-404d-bf3e-92799569a69b",
          "name": "venuesmanaged",
          "request": {
            "url": "http://api.foursquare.com/v2/venues/search?alt=%7B%7D&altAcc=%7B%7D&categoryId=%7B%7D&intent=%7B%7D&limit=%7B%7D&linkedId=%7B%7D&ll=%7B%7D&llAcc=%7B%7D&ne=%7B%7D&providerId=%7B%7D&query=%7B%7D&radius=%7B%7D&sw=%7B%7D&url=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/venues/managed"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31c4dca7-edb2-4e14-bb46-d37390f4137a"
            }
          ]
        },
        {
          "id": "a33b308a-e7bc-4d42-9d34-2be58facac13",
          "name": "venuessearch",
          "request": {
            "url": "http://api.foursquare.com/v2/venues/suggestcompletion?alt=%7B%7D&altAcc=%7B%7D&limit=%7B%7D&ll=%7B%7D&llAcc=%7B%7D&query=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/venues/search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99e03014-514e-4657-a57f-b1da54c8430e"
            }
          ]
        },
        {
          "id": "add7f54d-0b64-411b-aa5a-0ab87d283cac",
          "name": "venuessuggestcompletion",
          "request": {
            "url": "http://api.foursquare.com/v2/venues/timeseries?endAt=%7B%7D&startAt=%7B%7D&v=%7B%7D&venueId=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/venues/suggestcompletion"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d188bdd-310d-45d5-81bf-4fa5686b6ba6"
            }
          ]
        },
        {
          "id": "8e2c55b8-ebe6-47ef-af10-9b07598eaa2b",
          "name": "venuestimeseries",
          "request": {
            "url": "http://api.foursquare.com/v2/venues/trending?limit=%7B%7D&ll=%7B%7D&radius=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/venues/timeseries"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b039ca0a-191a-43b4-ad89-b065576631bf"
            }
          ]
        },
        {
          "id": "c4b51f1e-75cc-49a9-bf99-34c4616ce059",
          "name": "usersselfupdate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "venues/:VENUE_ID"
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
                  "id": "VENUE_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/users/self/update"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e5b9bc3-4c68-41d6-ba39-3e85b35650ed"
            }
          ]
        },
        {
          "id": "25bd60cd-48e9-4d28-b227-e4baa68d33fe",
          "name": "venuesvenue-idtips",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "venues/:VENUE_ID/edit"
              ],
              "query": [
                {
                  "key": "address",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "categoryId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "city",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "crossStreet",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ll",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "phone",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "state",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "twitter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "url",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "zip",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "VENUE_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/venues/{VENUE_ID}/tips"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "77157d78-6eae-42ad-98a0-785b54fe6086"
            }
          ]
        },
        {
          "id": "4c6dfe20-60b7-4c76-ac00-56f1b610f142",
          "name": "venuestrending",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "venues/:VENUE_ID/events"
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
                  "id": "VENUE_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/venues/trending"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "96a10b9c-390b-4d6b-96a2-776d1f013e8d"
            }
          ]
        },
        {
          "id": "651fddc0-7d43-4169-9e79-37069f975161",
          "name": "venuesvenue-idedit",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "venues/:VENUE_ID/flag"
              ],
              "query": [
                {
                  "key": "problem",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venueId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "VENUE_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/venues/{VENUE_ID}/edit"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ca4c852-f1a6-41ea-8d76-6d9b65bd6def"
            }
          ]
        }
      ]
    }
  ]
}