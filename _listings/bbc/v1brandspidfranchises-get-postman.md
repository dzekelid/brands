{
  "info": {
    "name": "BBC Nitro Get raw brand franchise",
    "_postman_id": "7c557fef-1ff2-4ab5-8b01-f8383b59a790",
    "description": "Get raw brand franchises",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Folder",
      "item": [
        {
          "id": "3776b22e-d2d2-4c9d-aec6-f5037f5177ab",
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
              "id": "6a48e70a-cd52-4ce0-aed5-80d35ca8b901"
            }
          ]
        }
      ]
    },
    {
      "name": "Availabilities",
      "item": [
        {
          "id": "a17d0820-a25f-4cf1-bde0-d3cede147ed1",
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
              "id": "baa9a79a-e98d-4c2d-87f6-942e48250871"
            }
          ]
        }
      ]
    },
    {
      "name": "Broadcasts",
      "item": [
        {
          "id": "587df8b8-6cb0-46a2-b8af-bf512dd8bb7d",
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
              "id": "7216f5d1-b1fb-4d16-beba-a3ee13f4c404"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "19cd214e-1caf-408d-b161-6bc70a3fe872",
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
              "id": "9a7aa32e-ad09-4c77-8fb9-b916194ee869"
            }
          ]
        }
      ]
    },
    {
      "name": "Images",
      "item": [
        {
          "id": "eeb68a7c-5923-46f5-86bb-ac8fa070e121",
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
              "id": "7f298732-4a43-4717-96cd-907feddd5211"
            }
          ]
        }
      ]
    },
    {
      "name": "Items",
      "item": [
        {
          "id": "b85184ad-e658-40fd-ac15-6bf6b0de90ff",
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
              "id": "e7fb84fb-4fdf-4971-a7f6-35047b44f19b"
            }
          ]
        }
      ]
    },
    {
      "name": "Master",
      "item": [
        {
          "id": "cd9737da-5274-4818-8b33-68b7d338ef0a",
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
              "id": "07d7d033-a1d6-4894-a51d-d203795bc701"
            }
          ]
        }
      ]
    },
    {
      "name": "People",
      "item": [
        {
          "id": "24a6f1d7-9181-4147-9771-e5ff127a5c4b",
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
              "id": "3ca85251-37ba-49e2-8a33-2489794cfa79"
            }
          ]
        }
      ]
    },
    {
      "name": "Pips",
      "item": [
        {
          "id": "dca6c018-cf74-4994-9dc3-1c7b173d20a7",
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
              "id": "3feca1d7-1813-4a3a-ba3f-675c7fb45e59"
            }
          ]
        }
      ]
    },
    {
      "name": "Programme",
      "item": [
        {
          "id": "523c5c0d-bcbe-4b1a-a1ed-cee9a07e7828",
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
              "id": "ec1e10b5-cdde-492d-8467-a6bc0858c631"
            }
          ]
        }
      ]
    },
    {
      "name": "Programmes",
      "item": [
        {
          "id": "523f0906-b699-4fc6-8ee1-ab2cc07676d1",
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
              "id": "dab3aba8-eac0-40ef-a2f7-b963570fdc98"
            }
          ]
        }
      ]
    },
    {
      "name": "Promotions",
      "item": [
        {
          "id": "ffeda7ae-d0c2-4ed1-9280-77f6d21ae25e",
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
              "id": "d6bd88c4-025e-4144-b305-63b36d46c020"
            }
          ]
        }
      ]
    },
    {
      "name": "Schedules",
      "item": [
        {
          "id": "4688ba6b-3782-4c3e-918c-41999268d7e7",
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
              "id": "c47ac9f0-5525-4588-b012-18476d9b94bd"
            }
          ]
        }
      ]
    },
    {
      "name": "Schema",
      "item": [
        {
          "id": "43295da7-9838-4405-af8c-dd7cd446bad7",
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
              "id": "eb05cdbc-c8b1-455b-95cd-7b4c6b216fd3"
            }
          ]
        }
      ]
    },
    {
      "name": "Services",
      "item": [
        {
          "id": "d9542b90-e26e-434c-9602-6a5d1640bb73",
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
              "id": "74446007-14b4-409a-9c93-d497f8e72a52"
            }
          ]
        }
      ]
    },
    {
      "name": "V1",
      "item": [
        {
          "id": "ccac6a23-c215-4d05-afe6-66077cb526aa",
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
              "id": "6b4bce3a-6e7f-4274-a759-c6e45265b645"
            }
          ]
        },
        {
          "id": "03dcfeec-f4f3-4a6c-82c2-2380112333e2",
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
              "id": "6c9ae3dc-9a4e-49bc-96dc-e9764affd8f1"
            }
          ]
        }
      ]
    }
  ]
}