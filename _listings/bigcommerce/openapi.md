swagger: "2.0"
x-collection-name: BigCommerce
x-complete: 1
info:
  title: BigCommerce API V3
  description: collection-of-requests-for-interacting-with-bigcommerces-v3-api
  version: 1.0.0
host: api.bigcommerce.com
basePath: /stores
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{store_hash}/v3/catalog/brands:
    get:
      summary: Retrieve brands
      description: ""
      operationId: V3CatalogBrandsByStoreHashGet
      x-api-path-slug: store-hashv3catalogbrands-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: page
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Brands
    delete:
      summary: Delete a brand or brands
      description: Delete one or more `Brand` objects from the BigCommerce Catalog
      operationId: V3CatalogBrandsByStoreHashDelete
      x-api-path-slug: store-hashv3catalogbrands-delete
      parameters:
      - in: query
        name: page_title
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Brand
      - Brands
    post:
      summary: Create a new brand
      description: ""
      operationId: V3CatalogBrandsByStoreHashPost
      x-api-path-slug: store-hashv3catalogbrands-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Brand
  /{store_hash}/v3/catalog/brands/{id}/image:
    post:
      summary: Upload an image for a brand
      description: ""
      operationId: V3CatalogBrandsImageByStoreHashAndIdPost
      x-api-path-slug: store-hashv3catalogbrandsidimage-post
      parameters:
      - in: path
        name: id
      - in: formData
        name: image_file
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Upload
      - Imagea
      - Brand
    delete:
      summary: Delete a brand image
      description: Delete a `Brand` image the BigCommerce Catalog
      operationId: V3CatalogBrandsImageByStoreHashAndIdDelete
      x-api-path-slug: store-hashv3catalogbrandsidimage-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Brand
      - Image
  /{store_hash}/v3/catalog/brands/{id}:
    get:
      summary: Retrieve a brand
      description: ""
      operationId: V3CatalogBrandsByStoreHashAndIdGet
      x-api-path-slug: store-hashv3catalogbrandsid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Brand
    put:
      summary: Update a brand
      description: ""
      operationId: V3CatalogBrandsByStoreHashAndIdPut
      x-api-path-slug: store-hashv3catalogbrandsid-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Brand
    delete:
      summary: Delete a brand
      description: ""
      operationId: V3CatalogBrandsByStoreHashAndIdDelete
      x-api-path-slug: store-hashv3catalogbrandsid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Brand