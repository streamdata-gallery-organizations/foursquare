{
  "info": {
    "name": "Foursquare Get Venues Tips",
    "_postman_id": "c5ab5a3f-ff4a-449a-94e7-65ec98916890",
    "description": "/venues/{VENUE_ID}/stats",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Campaigns",
      "item": [
        {
          "id": "f2e0dcb8-f19f-4fcc-a038-4b4cf5a3728f",
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
              "id": "5d318721-4eb5-4616-b54c-8bf84ef92264"
            }
          ]
        },
        {
          "id": "7f61bfdc-5d48-4a49-b75f-eec1c276b90d",
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
              "id": "bac2778c-8ba8-4351-a534-494efb2ad283"
            }
          ]
        },
        {
          "id": "5535468c-56eb-4f93-8e80-5614166f9237",
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
              "id": "4569718a-18cd-47ea-aebc-6b12d455a0b8"
            }
          ]
        },
        {
          "id": "ddeed645-400f-440f-b60d-81ebde1076f0",
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
              "id": "1053ab08-239e-4b03-aedd-dad188489446"
            }
          ]
        },
        {
          "id": "dfd85101-2f99-4488-84c2-2dfa46e544d6",
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
              "id": "e2c5b318-de58-47d9-9915-3836668978d6"
            }
          ]
        },
        {
          "id": "1e6e2c87-e909-4ec5-a5da-ad695a350876",
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
              "id": "f37d5d8b-e0ed-4e17-bb86-edb247bad6a8"
            }
          ]
        },
        {
          "id": "6721e784-94e9-46cd-900d-280f562bdc63",
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
              "id": "fc90d9dc-d2e2-4164-85b0-3981905b668a"
            }
          ]
        }
      ]
    },
    {
      "name": "Checkins",
      "item": [
        {
          "id": "bb13af32-c08f-4e1c-aad5-18ed0768475a",
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
              "id": "95690031-53c2-4e5f-84ba-d2f7c316a0f7"
            }
          ]
        },
        {
          "id": "cb84a54a-4ff6-432d-a887-00f555319250",
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
              "id": "548039be-da36-4f31-a322-a3b0e6367de8"
            }
          ]
        },
        {
          "id": "7b80d304-a391-4ebd-90b9-ad08d19c58b4",
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
              "id": "58097179-6976-4507-b7ba-ffccb9121713"
            }
          ]
        },
        {
          "id": "5b12662c-f9e4-49ac-adb4-88daa0c0bb54",
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
              "id": "a44b975e-9f92-4cbb-b1bd-87b63bd00f54"
            }
          ]
        },
        {
          "id": "553e7880-b907-4ba8-b00e-c34b943e308c",
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
              "id": "db083488-895c-4786-b007-10d61834b3b4"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "ec481ddb-37b0-46cd-af87-fb20b303e28d",
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
              "id": "b836d35c-b962-410c-a165-440d1b240b07"
            }
          ]
        },
        {
          "id": "3e4721b7-8d55-493a-95ab-dd4e8aaa74b7",
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
              "id": "77b3b80b-722a-4433-9625-455453c0486b"
            }
          ]
        },
        {
          "id": "d93837e3-2ee9-4c2f-88f0-5191bbe1f20f",
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
              "id": "1fff91d0-b842-4bfe-8355-f1753d45bbbb"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "46b2370c-a6d3-40c4-960f-72739e5b679c",
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
              "id": "2fca0f92-822c-41a1-bf47-d0f8a5704c54"
            }
          ]
        },
        {
          "id": "eaf4e9f8-e9f5-4141-a090-20a59008c243",
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
              "id": "0390c05b-94a0-410e-bf21-84d7c8e85cfa"
            }
          ]
        },
        {
          "id": "dbcc66b8-ce55-4088-b48f-2e059f8c7690",
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
              "id": "2ba2d1b2-739c-4d01-9636-4411c9560f1f"
            }
          ]
        },
        {
          "id": "adff9a65-8467-467a-82da-7bfab1012beb",
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
              "id": "aac81cd6-e7cd-4290-ad63-7bfa8484ce1a"
            }
          ]
        },
        {
          "id": "ddec0b6e-a0d4-47f3-9243-71155d308589",
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
              "id": "a83ee7ab-0479-4867-936f-4a7487178d35"
            }
          ]
        },
        {
          "id": "93b4eda8-f46c-4af7-977f-5d7f12b317f6",
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
              "id": "0ea9254e-ed68-4eb3-b9b1-93df1fdf6703"
            }
          ]
        },
        {
          "id": "b68b5d3f-4176-4912-8ae7-3fbf4e5d1716",
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
              "id": "11d4d184-9cf1-490e-803b-084497db121f"
            }
          ]
        },
        {
          "id": "fcfb00ce-1eec-460b-a657-1577a256f6d5",
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
              "id": "93382e0f-bf97-4ae7-bbd5-e404a6ebcafc"
            }
          ]
        },
        {
          "id": "976ffcad-383e-428c-80e4-dd1991b167d5",
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
              "id": "d1ff3d83-24bb-4ae1-a217-8dec9de66bb1"
            }
          ]
        },
        {
          "id": "3028c9f5-6d58-42ea-add6-cd7697904287",
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
              "id": "9a8f1415-161b-4ec9-99d3-3bc05163bd49"
            }
          ]
        },
        {
          "id": "d64ec960-b5fd-4c7f-bd29-d7424ea8ae7a",
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
              "id": "732e4d32-9921-4831-81bd-6b519bcbec7c"
            }
          ]
        },
        {
          "id": "34d03cae-b035-46db-86e5-83aaa5b488c3",
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
              "id": "e32cf99f-6e14-4621-af70-245ff0e611bb"
            }
          ]
        },
        {
          "id": "d2ae1742-20c3-4543-802c-0138dee7e57a",
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
              "id": "9f78dead-43a7-4346-a29a-085bcd66cc81"
            }
          ]
        },
        {
          "id": "916d2572-75b8-48cc-b2ad-dbfec72b3216",
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
              "id": "a9c7dbc2-91b9-464b-a415-6380cdad2b9b"
            }
          ]
        }
      ]
    },
    {
      "name": "Multi",
      "item": [
        {
          "id": "9e85daf0-b479-4b6e-832c-30645a7fb87d",
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
              "id": "56ae7146-e334-441f-956e-b5ae0f5e11ad"
            }
          ]
        }
      ]
    },
    {
      "name": "Pages",
      "item": [
        {
          "id": "880ea847-ecca-48ce-a4ec-585bae56a9a9",
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
              "id": "526b30d9-76ed-4f1d-8331-2c1abebbb454"
            }
          ]
        },
        {
          "id": "d5351c61-3110-48e8-98ad-74a1874e88df",
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
              "id": "735e28f1-cfac-443d-ac40-4b7b8481e245"
            }
          ]
        },
        {
          "id": "8520c7ac-b7ad-48d1-8c10-e6c726a37b8e",
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
              "id": "a6e25807-c0c5-46c9-a210-50cef10d1115"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "ee869fc6-b97a-4021-be63-c253a45f77e3",
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
              "id": "41104c12-baca-4654-865d-96c9824ff501"
            }
          ]
        },
        {
          "id": "c77a74f9-2914-4e9d-a8c6-a77e44c319d3",
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
              "id": "aaa01a64-9129-4298-b5fc-af85e063a0ce"
            }
          ]
        }
      ]
    },
    {
      "name": "Settings",
      "item": [
        {
          "id": "892b6d6c-9002-4949-b05a-7a44ddb258a0",
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
              "id": "25474c25-3c30-4e1a-99bb-69adba43c3a4"
            }
          ]
        },
        {
          "id": "ffe5d2e0-174f-4fb9-b877-cf91dd635d26",
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
              "id": "5859a50c-2bc4-4558-a864-481e461c2a91"
            }
          ]
        },
        {
          "id": "37737925-0025-41b5-b875-2dc68e0ed014",
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
              "id": "18c7dd28-f24d-4f1a-9a0f-d8c4bf696a07"
            }
          ]
        }
      ]
    },
    {
      "name": "Specials",
      "item": [
        {
          "id": "0b57b722-ed71-4ec2-b9e3-6e2ff175ec2b",
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
              "id": "8a06b817-6694-4a3e-bc32-0d0712701719"
            }
          ]
        },
        {
          "id": "765a1670-6f9e-4e4e-80ca-29fb58a85feb",
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
              "id": "2c8fee0b-054e-4c8f-b3a4-a6907d62770f"
            }
          ]
        },
        {
          "id": "4e026e1b-f11d-483f-b00a-65ec3e8ad5e9",
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
              "id": "0d99afc5-5ece-401a-8a22-ae43ff474913"
            }
          ]
        },
        {
          "id": "7f8b47ad-5a7e-464c-9f5a-0861ad7c6c39",
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
              "id": "828eac3b-51d6-4156-ab0a-ef4a0283ea72"
            }
          ]
        },
        {
          "id": "3053a145-5a7a-4bf2-bfe6-27dd5ad71582",
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
              "id": "8f665ae8-2ced-4889-aea4-d96c2533e4c5"
            }
          ]
        },
        {
          "id": "6ba720d2-7b22-475c-8455-a677729c6e4a",
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
              "id": "cbd10857-e265-4ea8-adfc-b62dd119c814"
            }
          ]
        },
        {
          "id": "1de05f81-6573-49c4-9eb4-6e287a6ca98f",
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
              "id": "679a27be-bda3-4d0a-b614-f74ce1321db9"
            }
          ]
        }
      ]
    },
    {
      "name": "Tips",
      "item": [
        {
          "id": "2e1c6018-a5ba-4e8b-bf0b-2469ea79b2a6",
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
              "id": "e906e951-88ec-455e-94c8-0792672b54e4"
            }
          ]
        },
        {
          "id": "9d1b188d-dbc6-42a1-9ebb-170b3dab7cab",
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
              "id": "6767129f-695a-45e7-a231-94c87d0b4a83"
            }
          ]
        },
        {
          "id": "ff07105e-b699-45cd-a72f-9660288e0575",
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
              "id": "f46f336a-9ce0-41df-a1da-79fef40e25c2"
            }
          ]
        },
        {
          "id": "cf922fbe-26a7-4aac-afe1-2fe19d3fc264",
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
              "id": "ad371a37-fe24-400e-891d-46741ff0cb9d"
            }
          ]
        },
        {
          "id": "5c3ff439-3896-4d76-b434-09adb3175ec8",
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
              "id": "8471e141-1793-4227-975b-547d4526fbe8"
            }
          ]
        },
        {
          "id": "c344fc1f-ad0f-4677-b2b3-7f398e0526eb",
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
              "id": "6d96ab36-2982-4fc6-ad32-9773bd649b15"
            }
          ]
        },
        {
          "id": "c4272c8e-8f45-4fc3-b61d-cb82f83b9d9c",
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
              "id": "f26f7181-6e0a-4bd0-8f8d-924407da42a4"
            }
          ]
        },
        {
          "id": "2f46332d-b354-4a71-89f8-eb4192ff4235",
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
              "id": "718761e2-87ff-49cf-8c46-bf6836050785"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "e6d555be-ffda-4772-8d09-c9db69ce53d4",
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
              "id": "82e8a89e-997e-4ba7-812c-21048100be91"
            }
          ]
        },
        {
          "id": "62b65039-4581-456b-a82d-a52fe75eb051",
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
              "id": "b44bcddd-f81d-4c7c-936a-bfe2d7ad1eb2"
            }
          ]
        },
        {
          "id": "e970becf-dd05-4edf-bf81-d5e2a83c4dab",
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
              "id": "7d5b3a14-a34f-4391-b5eb-7a4ae3efa238"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "96c9e963-41cb-4e75-bf44-f749a909105e",
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
              "id": "5d55e47d-c788-449d-92de-68984beb5f04"
            }
          ]
        },
        {
          "id": "f84b3f48-9897-4a08-9f58-bac2a94db5db",
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
              "id": "41eaead8-eaad-4760-a5a2-a3d673210956"
            }
          ]
        },
        {
          "id": "ab2354a4-0752-492b-9c86-1baa0e46a855",
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
              "id": "18b0d4c6-a57e-442e-9b57-d696e146a76c"
            }
          ]
        },
        {
          "id": "bd148bd7-ae25-4304-b5ea-41358d1d6eac",
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
              "id": "ad86fe23-0975-4bf1-8fcc-116a46975d65"
            }
          ]
        },
        {
          "id": "cbb22b77-8c13-4715-b1f6-d125c4a817d3",
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
              "id": "51dd15d2-4611-474e-bace-7ee5af9a6bae"
            }
          ]
        },
        {
          "id": "d1eabfdc-0fb2-4886-b837-919047279e09",
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
              "id": "b0f176c8-53fd-488e-af66-ad8f90cee65b"
            }
          ]
        },
        {
          "id": "359aaca3-51b0-473f-8703-f9f203c0febc",
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
              "id": "8bd7748d-c25a-4f7a-9f05-3ff806c0ea8d"
            }
          ]
        },
        {
          "id": "ec92cb8d-a07d-408a-9f6c-93b51a7f15e5",
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
              "id": "10d95ebf-bcaf-4310-9d33-9cd278682c70"
            }
          ]
        },
        {
          "id": "6bc14cdd-852e-4921-8426-d259d9afff3a",
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
              "id": "455dbec8-8a44-4a7b-98b2-519281e021a3"
            }
          ]
        },
        {
          "id": "f35aea8c-c3e8-4727-a425-fce01265b35c",
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
              "id": "d1a3e298-4dd6-48c0-b911-a0d8f6e39ef6"
            }
          ]
        },
        {
          "id": "663ab739-0577-4d11-ad32-dbeec8938888",
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
              "id": "b3e7013c-47ee-4258-8a7a-1c6e5a046039"
            }
          ]
        },
        {
          "id": "849ae9be-9d67-432b-93b3-8b78226904fa",
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
              "id": "b948999f-dd87-422c-b3cf-e4358af5e393"
            }
          ]
        },
        {
          "id": "f814a395-5a5d-4d33-9a7a-ab85d909cd54",
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
              "id": "84d2981e-9d2c-4814-954a-17e24917bf63"
            }
          ]
        },
        {
          "id": "9f9753d5-4b5d-4dc6-8aeb-22a6911196f2",
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
              "id": "3c56559d-ce6a-473f-880a-7f587d7218ea"
            }
          ]
        },
        {
          "id": "4d4f1591-ce1c-4f8c-bae6-07c78bcc78a1",
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
              "id": "a0c5f728-7ec5-4d0b-9f01-c1729d56601d"
            }
          ]
        },
        {
          "id": "ffad2b2c-89a4-4c7f-b7a1-f8ad1d342924",
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
              "id": "e1991717-f879-4ac1-bf24-89020f2f4573"
            }
          ]
        },
        {
          "id": "0a1c8559-10e7-4d30-a746-71c3409412e5",
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
              "id": "bd053cd6-71d6-42d6-a0ce-4edf903acd9b"
            }
          ]
        },
        {
          "id": "ff559cfe-93dc-4ae0-82ef-99f526e04068",
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
              "id": "b8ad609e-fcec-4aab-9f1b-a46830b4c238"
            }
          ]
        },
        {
          "id": "0d155f8c-ae77-4431-8418-572796295093",
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
              "id": "ff279b24-713d-4753-acc6-da752724eaf2"
            }
          ]
        },
        {
          "id": "77fe63eb-f33e-49fa-a99f-7bc1d7918480",
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
              "id": "f4a19523-5054-442e-92cf-8085c7394289"
            }
          ]
        }
      ]
    },
    {
      "name": "Venuegroups",
      "item": [
        {
          "id": "68919d94-eebd-4d38-8a8c-0cd6a5f6c562",
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
              "id": "b1deb2d8-7132-450b-8926-c8bd0dca1db5"
            }
          ]
        },
        {
          "id": "8046545b-202e-40a8-a4dd-86ecd6260b1b",
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
              "id": "c024305c-9ab4-4d2d-a77f-da1ddf9dc1f2"
            }
          ]
        },
        {
          "id": "5d74dfdf-1ad1-4242-8a5c-ddb054c38321",
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
              "id": "378e8a46-5a66-4629-8660-eb0ffa154191"
            }
          ]
        },
        {
          "id": "4d30d0b1-7291-46fa-853b-452e235128c6",
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
              "id": "f1fc4da2-b85e-4e4f-9e8a-235cda8b3003"
            }
          ]
        },
        {
          "id": "bfcdb467-5957-47c1-84b8-5b4a290400c5",
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
              "id": "ffe0c8d1-979a-4927-9d46-f295ef642837"
            }
          ]
        },
        {
          "id": "98d8e50f-7986-48f7-b3b2-d3700202002e",
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
              "id": "948254a9-b548-4f25-9168-57ab1f0ce8c8"
            }
          ]
        }
      ]
    },
    {
      "name": "Venues",
      "item": [
        {
          "id": "b7180608-fb82-4490-a22d-762c8ec8d2b7",
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
              "id": "1f8000db-3dc1-47ed-bcaa-c35d1d251830"
            }
          ]
        },
        {
          "id": "9d1167ec-2765-42db-b086-28798556301d",
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
              "id": "e655fa2e-ce37-42a5-a9c7-65adef86c98d"
            }
          ]
        },
        {
          "id": "3f8d9ab8-a3a1-4562-bf8e-88d2c4c49b3e",
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
              "id": "d1aaffeb-19d5-45cc-8b37-9724bba14849"
            }
          ]
        },
        {
          "id": "064a292e-323f-4853-ade3-fed8307389aa",
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
              "id": "186d2103-c6c3-4beb-a8f7-f7557baefb8f"
            }
          ]
        },
        {
          "id": "27d1cadb-b166-4048-a1e7-828f7edba936",
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
              "id": "21a6413e-de51-4087-bb7c-a65cab1b512d"
            }
          ]
        },
        {
          "id": "859c30dc-3163-4ff7-b171-0c314805a59f",
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
              "id": "0dd7e13c-0840-4d17-bf27-9791bdea1492"
            }
          ]
        },
        {
          "id": "e3474cc8-ba1d-4c37-aac6-760b6296dd02",
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
              "id": "7563d324-efeb-43f7-ad82-42452570aa52"
            }
          ]
        },
        {
          "id": "c8753ebe-a89d-452f-887a-75f3cc244836",
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
              "id": "daee4b7b-5d57-4ed9-8117-1538ed03482e"
            }
          ]
        },
        {
          "id": "4953d79b-24af-404a-96c7-d4671291b8de",
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
              "id": "785e99bc-2797-4de2-ba30-d5bc4364b7f2"
            }
          ]
        },
        {
          "id": "fc155c87-1fc0-4dc3-8c52-c9b9425ca61e",
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
              "id": "b1c071de-470a-4e48-956d-8a6328e252de"
            }
          ]
        },
        {
          "id": "815c4180-a8f1-4126-8e44-122e698601bd",
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
              "id": "67d07aab-e3f6-48f6-816b-b65cf396a4d4"
            }
          ]
        },
        {
          "id": "ee11d0b8-9c5e-4f5f-90d8-c5d14e38c678",
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
              "id": "1ca441f8-49af-49df-9cac-5e05cbdb6c3f"
            }
          ]
        },
        {
          "id": "6a559d3b-d55d-4e95-8864-f9288839693f",
          "name": "venuesvenue-idevents",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "venues/:VENUE_ID/herenow"
              ],
              "query": [
                {
                  "key": "afterTimestamp",
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
            "description": "/venues/{VENUE_ID}/events"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a5bbd2c-4173-4926-af8a-306342fc94f5"
            }
          ]
        },
        {
          "id": "b7e5f668-cd47-4c7a-b0fe-a6b0705d7589",
          "name": "venuesvenue-idherenow",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "venues/:VENUE_ID/links"
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
            "description": "/venues/{VENUE_ID}/herenow"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb70d015-32ac-4843-8fa9-ec16bdf00e14"
            }
          ]
        },
        {
          "id": "93782b1b-9fbc-4271-ade7-c95df4e9ffef",
          "name": "venuesvenue-idlinks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "venues/:VENUE_ID/listed"
              ],
              "query": [
                {
                  "key": "group",
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
            "description": "/venues/{VENUE_ID}/links"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9995da4-93c9-42c7-8732-266ca096325e"
            }
          ]
        },
        {
          "id": "a9d923ec-4c31-4e8f-b1d4-5ee35812f873",
          "name": "venuesvenue-idflag",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "venues/:VENUE_ID/marktodo"
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
            "description": "/venues/{VENUE_ID}/flag"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90b38cb5-0189-4aa6-bec1-79c4fc1b21d5"
            }
          ]
        },
        {
          "id": "bed1a79a-b085-41a3-b716-289675203270",
          "name": "venuesvenue-idlisted",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "venues/:VENUE_ID/menu"
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
            "description": "/venues/{VENUE_ID}/listed"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6e30b96-9428-4661-9af3-afeb1ddc2d75"
            }
          ]
        },
        {
          "id": "667645ae-261a-4631-8002-7582ef31c440",
          "name": "venuesvenue-idmenu",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "venues/:VENUE_ID/photos"
              ],
              "query": [
                {
                  "key": "group",
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
            "description": "/venues/{VENUE_ID}/menu"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e46e764-280a-4541-8f9c-9fd588f0bb80"
            }
          ]
        },
        {
          "id": "20951e5f-0b83-4e11-b718-adbeb5952918",
          "name": "venuesvenue-idmarktodo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "venues/:VENUE_ID/proposeedit"
              ],
              "query": [
                {
                  "key": "address",
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
                  "key": "primaryCategoryId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "state",
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
            "description": "/venues/{VENUE_ID}/marktodo"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a411321-000d-4bf5-a1b1-e1711c452dba"
            }
          ]
        },
        {
          "id": "3586778a-78d1-406a-b698-a83b324b17a9",
          "name": "venuesvenue-idphotos",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "venues/:VENUE_ID/similar"
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
            "description": "/venues/{VENUE_ID}/photos"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "438d33b0-c750-40d7-b2ea-7b9de8fccfa5"
            }
          ]
        },
        {
          "id": "0c32943c-d0d6-4ac5-9322-5375793bacbd",
          "name": "venuesvenue-idsimilar",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "venues/:VENUE_ID/stats"
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
            "description": "/venues/{VENUE_ID}/similar"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e777e924-22fc-4638-9919-e25665d989f7"
            }
          ]
        },
        {
          "id": "39572fec-a0e7-4312-b385-0afe6b1892f6",
          "name": "venuesvenue-idstats",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "venues/:VENUE_ID/tips"
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
            "description": "/venues/{VENUE_ID}/stats"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aae6c483-8993-4128-9c9b-d24fb1f6147e"
            }
          ]
        }
      ]
    }
  ]
}