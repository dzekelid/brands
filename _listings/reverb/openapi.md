swagger: "2.0"
x-collection-name: Reverb
x-complete: 1
info:
  title: reverb
  description: reverb
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /my/follows/brands/{slug}:
    delete:
      summary: Delete My Follows Brands Slug
      description: Delete my follows brands slug.
      operationId: deleteMyFollowsBrandsSlug
      x-api-path-slug: myfollowsbrandsslug-delete
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Brands
      - Slug
    get:
      summary: Get My Follows Brands Slug
      description: Get my follows brands slug.
      operationId: getMyFollowsBrandsSlug
      x-api-path-slug: myfollowsbrandsslug-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Brands
      - Slug
    post:
      summary: Post My Follows Brands Slug
      description: Post my follows brands slug.
      operationId: postMyFollowsBrandsSlug
      x-api-path-slug: myfollowsbrandsslug-post
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Brands
      - Slug