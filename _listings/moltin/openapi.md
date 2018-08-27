swagger: "2.0"
x-collection-name: moltin
x-complete: 1
info:
  title: Moltin
  description: -welcomethis-is-a-place-to-put-general-notes-and-extra-information-for-internal-use-to-get-started-designingdocumenting-this-api-select-a-version-on-the-left-
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/brands/{brandID}:
    get:
      summary: Get a Brand
      description: Get a brand.
      operationId: V2BrandsByBrandIDGet
      x-api-path-slug: v2brandsbrandid-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      - in: query
        name: include
      responses:
        200:
          description: Successful response
      tags:
      - Brands
    put:
      summary: Update a Brand
      description: Update a brand.
      operationId: V2BrandsByBrandIDPut
      x-api-path-slug: v2brandsbrandid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Brands
    delete:
      summary: Delete a Brand
      description: Delete a brand.
      operationId: V2BrandsByBrandIDDelete
      x-api-path-slug: v2brandsbrandid-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Brands
  /v2/brands/{brandID}/relationships/parent:
    put:
      summary: Update Parent Brand Relationship
      description: Update parent brand relationship.
      operationId: V2BrandsRelationshipsParentByBrandIDPut
      x-api-path-slug: v2brandsbrandidrelationshipsparent-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Brands
      - Relationship
    post:
      summary: Create Parent Brand Relationship
      description: Create parent brand relationship.
      operationId: V2BrandsRelationshipsParentByBrandIDPost
      x-api-path-slug: v2brandsbrandidrelationshipsparent-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Brands
      - Relationship
    delete:
      summary: Delete Parent Brand Relationship
      description: Delete parent brand relationship.
      operationId: V2BrandsRelationshipsParentByBrandIDDelete
      x-api-path-slug: v2brandsbrandidrelationshipsparent-delete
      parameters:
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Brands
      - Relationship
  /v2/products/{productID}/relationships/brands:
    delete:
      summary: Delete Products <=> Brands Relationships
      description: Here you can delete a relationship between a `Product` and `Brand`'s.
        Only those relationshops to `Brand`'s specified in the paylaod will be removed.
      operationId: V2ProductsRelationshipsBrandsByProductIDDelete2
      x-api-path-slug: v2productsproductidrelationshipsbrands-delete
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Brands
      - Relationships
    put:
      summary: Update Product <=> Brands Relationships
      description: Here you can set relations `Brand`'s to a product. The result of
        this request will set relationships between product and the specified brnads
        in teh payload and remove any other relations the product had with brands.
      operationId: V2ProductsRelationshipsBrandsByProductIDPut
      x-api-path-slug: v2productsproductidrelationshipsbrands-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Brandss
      - Relationships
    post:
      summary: Create Product <=> Brands Relationships
      description: Here you can add `Brand`'s to a product. The `Brand`'s found in
        the payload will be added to any other relationships to `Brand`'s present.
      operationId: V2ProductsRelationshipsBrandsByProductIDPost
      x-api-path-slug: v2productsproductidrelationshipsbrands-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Brandss
      - Relationships
  /v2/brands/{brandID}/relationships/children:
    put:
      summary: Update Child Brand Relationship
      description: Update child brand relationship.
      operationId: V2BrandsRelationshipsChildrenByBrandIDPut
      x-api-path-slug: v2brandsbrandidrelationshipschildren-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Brands
      - Relationship
    post:
      summary: Create Child Brand Relationship
      description: Create child brand relationship.
      operationId: V2BrandsRelationshipsChildrenByBrandIDPost
      x-api-path-slug: v2brandsbrandidrelationshipschildren-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Brands
      - Relationship
    delete:
      summary: Update Child Brand Relationship Copy
      description: Update child brand relationship copy.
      operationId: V2BrandsRelationshipsChildrenByBrandIDDelete
      x-api-path-slug: v2brandsbrandidrelationshipschildren-delete
      parameters:
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Brands
      - Relationship
      - Copy
  /v2/brands/tree:
    get:
      summary: Get a Brand tree
      description: Get a brand tree.
      operationId: V2BrandsTreeGet
      x-api-path-slug: v2brandstree-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Brands
      - Tree
  /v2/brands/attributes:
    get:
      summary: Get Brand Attributes
      description: Get brand attributes.
      operationId: V2BrandsAttributesGet
      x-api-path-slug: v2brandsattributes-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Brands
      - Attributes
  /v2/brands:
    get:
      summary: Get a list of Brands
      description: Get a list of brands.
      operationId: V2BrandsGet
      x-api-path-slug: v2brands-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Brands
    post:
      summary: Create a Brand
      description: Create a brand.
      operationId: V2BrandsPost
      x-api-path-slug: v2brands-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Brands
  /v2/brands/{brandID}/relationships/brands:
    post:
      summary: Create Brand Relationships
      description: Create brand relationships.
      operationId: V2BrandsRelationshipsBrandsByBrandIDPost
      x-api-path-slug: v2brandsbrandidrelationshipsbrands-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Brands
      - Relationships