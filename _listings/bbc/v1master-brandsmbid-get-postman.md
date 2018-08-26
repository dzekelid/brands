{
  "info": {
    "name": "BBC Nitro Get raw masterbrand",
    "_postman_id": "06c45290-3d2a-4f72-9af3-0d64dd500b19",
    "description": "Get raw masterbrand",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Folder",
      "item": [
        {
          "id": "42ed51fc-419c-4d03-941d-b2fe08cf3046",
          "name": "getAPI",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get API definition"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61ea99d5-cca3-40f9-bd30-9277385d3750"
            }
          ]
        }
      ]
    },
    {
      "name": "Availabilities",
      "item": [
        {
          "id": "51a7b71f-3951-49b2-8b57-f20b03346b3b",
          "name": "listAvailability",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/availabilities?availability=%7B%7D&debug=%7B%7D&descendants_of=%7B%7D&media_set=%7B%7D&page=%7B%7D&page_size=%7B%7D&sort=%7B%7D&sort_direction=%7B%7D&territory=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Discover details of on-demand availability for programmes and their versions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df43edb5-73ca-4799-ab6c-df40c874a1b2"
            }
          ]
        }
      ]
    },
    {
      "name": "Broadcasts",
      "item": [
        {
          "id": "ee6dce52-0cf1-45ba-8c33-9d0faf62e9e1",
          "name": "listBroadcasts",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/broadcasts?authority=%7B%7D&descendants_of=%7B%7D&end_from=%7B%7D&end_to=%7B%7D&format=%7B%7D&genre=%7B%7D&id=%7B%7D&item=%7B%7D&mixin=%7B%7D&page=%7B%7D&page_size=%7B%7D&people=%7B%7D&pid=%7B%7D&q=%7B%7D&schedule_day=%7B%7D&schedule_day_from=%7B%7D&schedule_day_to=%7B%7D&service_master_brand=%7B%7D&sid=%7B%7D&sort=%7B%7D&sort_direction=%7B%7D&start_from=%7B%7D&start_to=%7B%7D&version=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetch metadata about linear Broadcasts and Services, allowing the generation of Television and Radio schedules and other datasets for broadcast items. Use /schedules instead of this feed as it is more efficient. Broadcasts will be deprecated in the future."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93c7ad24-8b74-448c-8abf-66c8f9d3a704"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "1e30ed19-7d87-47d2-80fc-52a19a157042",
          "name": "listGroups",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/groups?embargoed=%7B%7D&for_descendants_of=%7B%7D&for_programme=%7B%7D&group=%7B%7D&group_type=%7B%7D&member=%7B%7D&mixin=%7B%7D&page=%7B%7D&page_size=%7B%7D&partner_id=%7B%7D&partner_pid=%7B%7D&pid=%7B%7D&q=%7B%7D&sort=%7B%7D&sort_direction=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Long-lived curated collections of programmes and more, including Collections, Seasons, Franchises and Galleries"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "767ccc57-7bdb-4dc8-b221-59befdf956ac"
            }
          ]
        }
      ]
    },
    {
      "name": "Images",
      "item": [
        {
          "id": "3dd2d3f9-f51c-4bd3-98f9-544cb508ea3b",
          "name": "listImages",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/images?embargoed=%7B%7D&group=%7B%7D&image_type=%7B%7D&is_alternate_image_for=%7B%7D&is_image_for=%7B%7D&page=%7B%7D&page_size=%7B%7D&partner_id=%7B%7D&partner_pid=%7B%7D&pid=%7B%7D&q=%7B%7D&sort=%7B%7D&sort_direction=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Find metadata for images, particularly those in galleries"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8dd4bbb-8890-4d08-b9dc-2b9d0a43612e"
            }
          ]
        }
      ]
    },
    {
      "name": "Items",
      "item": [
        {
          "id": "cee63b3b-cbd4-4bb3-b3f0-e3dcbbb780b5",
          "name": "listItems",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/items?authority=%7B%7D&id=%7B%7D&id_type=%7B%7D&item_type=%7B%7D&mixin=%7B%7D&page=%7B%7D&page_size=%7B%7D&partner_id=%7B%7D&partner_pid=%7B%7D&people=%7B%7D&pid=%7B%7D&programme=%7B%7D&q=%7B%7D&segment_event=%7B%7D&sort=%7B%7D&sort_direction=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Look inside programmes to find segments: chapters, tracks and more"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0825710-60a4-4701-b62f-80ebb67ebdc3"
            }
          ]
        }
      ]
    },
    {
      "name": "Master",
      "item": [
        {
          "id": "3a29ca63-cf22-423f-9a14-df273c0f6543",
          "name": "listMasterbrands",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/master_brands?mid=%7B%7D&mixin=%7B%7D&page=%7B%7D&page_size=%7B%7D&partner_id=%7B%7D&partner_pid=%7B%7D&q=%7B%7D&sort=%7B%7D&sort_direction=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all Master Brands"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "32e18100-0283-4fbc-802f-53877a41b384"
            }
          ]
        }
      ]
    },
    {
      "name": "People",
      "item": [
        {
          "id": "1cd4f4ef-681f-4e8b-bb67-492df806521d",
          "name": "listPeople",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/people?authority=%7B%7D&has_external_id=%7B%7D&id=%7B%7D&id_type=%7B%7D&page=%7B%7D&page_size=%7B%7D&partner_id=%7B%7D&partner_pid=%7B%7D&pid=%7B%7D&programme=%7B%7D&q=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The People feed allows you to search for the people and groups that contribute to programmes. This is the starting point for cast and crew credits, as well as finding contributors using external IDs (such as Wikipedia URLs)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c947197d-2614-4231-86a0-95c642e32c2a"
            }
          ]
        }
      ]
    },
    {
      "name": "Pips",
      "item": [
        {
          "id": "cb57539f-9181-4dba-a95a-9fc0115a1d8f",
          "name": "listPips",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/pips?page=%7B%7D&page_size=%7B%7D&q=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Look inside pips entities"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "675831a1-2895-4e17-9e3d-147a353fe518"
            }
          ]
        }
      ]
    },
    {
      "name": "Programme",
      "item": [
        {
          "id": "9801d6db-e68e-4359-8be1-477e4cfc7320",
          "name": "listProgrammeDetails",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/programme_details?page=%7B%7D&page_size=%7B%7D&partner_pid=%7B%7D&pid=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Exposes programme information for a single pid"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04bef040-f026-4e0d-a6cc-36913e963a4a"
            }
          ]
        }
      ]
    },
    {
      "name": "Programmes",
      "item": [
        {
          "id": "4af9e4a8-f8af-478b-ae56-b068414c98ab",
          "name": "listProgrammes",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/programmes?audio_described=%7B%7D&availability=%7B%7D&availability_entity_type=%7B%7D&availability_from=%7B%7D&availability_type=%7B%7D&children_of=%7B%7D&descendants_of=%7B%7D&duration=%7B%7D&embargoed=%7B%7D&entity_type=%7B%7D&format=%7B%7D&genre=%7B%7D&group=%7B%7D&initial_letter=%7B%7D&initial_letter_end=%7B%7D&initial_letter_start=%7B%7D&initial_letter_strict=%7B%7D&item=%7B%7D&master_brand=%7B%7D&media_set=%7B%7D&media_type=%7B%7D&mixin=%7B%7D&page=%7B%7D&page_size=%7B%7D&partner_id=%7B%7D&partner_pid=%7B%7D&payment_type=%7B%7D&people=%7B%7D&pid=%7B%7D&promoted_for=%7B%7D&q=%7B%7D&signed=%7B%7D&sort=%7B%7D&sort_direction=%7B%7D&tag_name=%7B%7D&tag_scheme=%7B%7D&tleo=%7B%7D&version=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetch metadata about Programmes (brands, series, episodes, clips). By applying different filter restrictions this feed can be used in many ways, for example to retrieve all series belonging to a brand, all the episodes and/or clips for a specific series, or any TLEO objects for a masterbrand. Other filters permit restricting to specific formats and/or genres, and you can request specific versions (for example Signed or Audio-Described). Parameters may be combined in any way suitable for your application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "03c5d994-a5e4-4bba-bca5-4b508dbf2f29"
            }
          ]
        }
      ]
    },
    {
      "name": "Promotions",
      "item": [
        {
          "id": "07e36d68-b2dc-41f6-82af-8d2e7d321752",
          "name": "listPromotions",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/promotions?context=%7B%7D&mixin=%7B%7D&page=%7B%7D&page_size=%7B%7D&partner_id=%7B%7D&partner_pid=%7B%7D&pid=%7B%7D&promoted_by=%7B%7D&promoted_for=%7B%7D&q=%7B%7D&status=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Details of short-term editorially curated \"promotions\", for instance those programmes featured on iPlayer today"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b88194eb-21a4-4605-9166-b507420f3138"
            }
          ]
        }
      ]
    },
    {
      "name": "Schedules",
      "item": [
        {
          "id": "990609b6-ad4d-46f9-b957-49ef21c3e14c",
          "name": "listSchedules",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/schedules?authority=%7B%7D&descendants_of=%7B%7D&end_from=%7B%7D&end_to=%7B%7D&format=%7B%7D&genre=%7B%7D&group=%7B%7D&id=%7B%7D&id_type=%7B%7D&item=%7B%7D&mixin=%7B%7D&page=%7B%7D&page_size=%7B%7D&partner_id=%7B%7D&partner_pid=%7B%7D&people=%7B%7D&pid=%7B%7D&q=%7B%7D&repeat=%7B%7D&schedule_day=%7B%7D&schedule_day_from=%7B%7D&schedule_day_to=%7B%7D&service_master_brand=%7B%7D&sid=%7B%7D&sort=%7B%7D&sort_direction=%7B%7D&start_from=%7B%7D&start_to=%7B%7D&version=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Dates, Times, Schedules: when and where are programmes being shown?"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42bed158-213d-412e-8474-726b79b36505"
            }
          ]
        }
      ]
    },
    {
      "name": "Schema",
      "item": [
        {
          "id": "4617c16c-9662-4dad-ab23-537f46724ffc",
          "name": "getXSD",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/schema",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Schema definition"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f6fa3a6-465f-4985-a23c-67447f9d729d"
            }
          ]
        }
      ]
    },
    {
      "name": "Services",
      "item": [
        {
          "id": "87296985-0154-4e7c-87b1-3549a12d4099",
          "name": "listServices",
          "request": {
            "url": "http://programmes.api.bbc.com/nitro/api/services?end_from=%7B%7D&end_to=%7B%7D&mid=%7B%7D&page=%7B%7D&page_size=%7B%7D&partner_id=%7B%7D&partner_pid=%7B%7D&q=%7B%7D&service_type=%7B%7D&sid=%7B%7D&start_from=%7B%7D&start_to=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The services feed exposes the linear broadcast \"services\" from PIPs. These are the actual services which broadcast programmes (eg bbc_one_oxford is the service for BBC One in Oxford)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41237c71-eca3-436f-b0c6-d1545b0380e5"
            }
          ]
        }
      ]
    },
    {
      "name": "V1",
      "item": [
        {
          "id": "8863f58b-0182-449f-a5e8-4460b0891214",
          "name": "Get_Raw_brand",
          "request": {
            "url": {
              "protocol": "http",
              "host": "programmes.api.bbc.com",
              "path": [
                "nitro",
                "api",
                "v1/brands/:pid"
              ],
              "variable": [
                {
                  "id": "pid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get raw brand"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "568eef23-85fd-44b5-97b9-15221bf2509c"
            }
          ]
        },
        {
          "id": "2f3738b1-951a-43a9-b002-2ff2d01e3602",
          "name": "Get_Raw_brand franchises",
          "request": {
            "url": {
              "protocol": "http",
              "host": "programmes.api.bbc.com",
              "path": [
                "nitro",
                "api",
                "v1/brands/:pid/franchises/"
              ],
              "variable": [
                {
                  "id": "pid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get raw brand franchises"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "492d649e-aa0b-4c88-ab30-7447093a2ea2"
            }
          ]
        },
        {
          "id": "a36537bb-380f-4ac5-92a4-b4a3b90f4a25",
          "name": "Get_Raw_episode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "programmes.api.bbc.com",
              "path": [
                "nitro",
                "api",
                "v1/episodes/:pid"
              ],
              "variable": [
                {
                  "id": "pid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get raw episode"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36ac344a-133b-4537-b7ad-54539cbe053d"
            }
          ]
        },
        {
          "id": "fefd4e65-8c2f-4ea1-83e9-3bce580292ad",
          "name": "Get_Raw_ancestors",
          "request": {
            "url": {
              "protocol": "http",
              "host": "programmes.api.bbc.com",
              "path": [
                "nitro",
                "api",
                "v1/episodes/:pid/ancestors/"
              ],
              "variable": [
                {
                  "id": "pid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get raw ancestors"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "51ad001f-0ebd-4da7-9852-15be40f1e301"
            }
          ]
        },
        {
          "id": "5a9963c5-d357-48c1-a618-72bf98f098f9",
          "name": "Get_Raw_formats",
          "request": {
            "url": {
              "protocol": "http",
              "host": "programmes.api.bbc.com",
              "path": [
                "nitro",
                "api",
                "v1/episodes/:pid/formats/"
              ],
              "variable": [
                {
                  "id": "pid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get raw formats"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9581320f-4ead-4534-a90d-5ccc3ac32cb8"
            }
          ]
        },
        {
          "id": "93476a3d-db5a-431e-a82b-e1c0f9b77261",
          "name": "Get_Raw_genre_groups",
          "request": {
            "url": {
              "protocol": "http",
              "host": "programmes.api.bbc.com",
              "path": [
                "nitro",
                "api",
                "v1/episodes/:pid/genre_groups/"
              ],
              "variable": [
                {
                  "id": "pid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get raw genre groups"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "129e8a2b-6ad4-4789-8caa-cadcdf3af357"
            }
          ]
        },
        {
          "id": "14b318c2-a83f-41bf-baa3-0189f88fbf7d",
          "name": "Get_Raw_image",
          "request": {
            "url": {
              "protocol": "http",
              "host": "programmes.api.bbc.com",
              "path": [
                "nitro",
                "api",
                "v1/images/:pid"
              ],
              "variable": [
                {
                  "id": "pid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get raw image"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf0d4a3b-ca75-499d-b2a2-8b20aa03007a"
            }
          ]
        },
        {
          "id": "a8b1a513-0ccc-45e3-9280-4ec8d76f2889",
          "name": "Get_Raw_masterbrand",
          "request": {
            "url": {
              "protocol": "http",
              "host": "programmes.api.bbc.com",
              "path": [
                "nitro",
                "api",
                "v1/master_brands/:mbid"
              ],
              "variable": [
                {
                  "id": "mbid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get raw masterbrand"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f42c576-367c-499a-a690-5541500d924a"
            }
          ]
        }
      ]
    }
  ]
}