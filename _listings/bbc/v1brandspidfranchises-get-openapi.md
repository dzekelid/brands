---
swagger: "2.0"
x-collection-name: BBC
x-complete: 0
info:
  title: BBC Nitro Get raw brand franchise
  description: Get raw brand franchises
  termsOfService: http://www.bbc.co.uk/terms/
  contact:
    name: Open Nitro Project
    url: http://developer.bbc.co.uk/
    email: nitro@bbc.co.uk
  version: 1.0.0
host: programmes.api.bbc.com
basePath: /nitro/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /master_brands:
    get:
      summary: List all Master Brands
      description: List all Master Brands
      operationId: listMasterbrands
      x-api-path-slug: master-brands-get
      parameters:
      - in: query
        name: mid
        description: filter for subset of masterbrands that have given identifier
      - in: query
        name: mixin
        description: 'Mixins:* images: mixin to add image information for a masterbrand'
      - in: query
        name: page
        description: which page of results to return
      - in: query
        name: page_size
        description: number of results in each page
      - in: query
        name: partner_id
        description: filter for masterbrands by partner ID
      - in: query
        name: partner_pid
        description: filter for masterbrands by partner PID
      - in: query
        name: q
        description: filter for subset of masterbrands matching supplied keyword/phrase
          (boolean operators permitted)
      - in: query
        name: sort
        description: 'Sorts:* mid: sort by mid, ascending'
      - in: query
        name: sort_direction
        description: Sort direction
      responses:
        200:
          description: OK
      tags:
      - Master
      - Brands
  /v1/brands/{pid}:
    get:
      summary: Get raw brand
      description: Get raw brand
      operationId: Get_Raw_brand
      x-api-path-slug: v1brandspid-get
      parameters:
      - in: path
        name: pid
      responses:
        200:
          description: OK
      tags:
      - V1
      - Brands
      - Pid
  /v1/brands/{pid}/franchises/:
    get:
      summary: Get raw brand franchise
      description: Get raw brand franchises
      operationId: Get_Raw_brand franchises
      x-api-path-slug: v1brandspidfranchises-get
      parameters:
      - in: path
        name: pid
      responses:
        200:
          description: OK
      tags:
      - V1
      - Brands
      - Pid
      - Franchises
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