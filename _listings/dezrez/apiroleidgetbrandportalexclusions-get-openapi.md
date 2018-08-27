---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get all brands with details for an agency
  version: 1.0.0
  description: Get all brands with details for an agency.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/branding/getallbrands:
    get:
      summary: Get all brands with details for an agency
      description: Get all brands with details for an agency.
      operationId: Branding_GetAllBrandsForAgency
      x-api-path-slug: apibrandinggetallbrands-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Brands
      - Detailsan
      - Agency
  /api/role/{id}/getbrandportalexclusions:
    get:
      summary: Get all brands with details for an agency
      description: Get all brands with details for an agency.
      operationId: Role_GetBrandPortalExclusionsByid
      x-api-path-slug: apiroleidgetbrandportalexclusions-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Brands
      - Detailsan
      - Agency
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