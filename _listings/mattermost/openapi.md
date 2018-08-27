swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost
  version: 1.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /brand/image:
    get:
      summary: Get brand image
      description: |-
        Get the previously uploaded brand image. Returns 404 if no brand image has been uploaded.
        ##### Permissions
        No permission required.
      operationId: get-the-previously-uploaded-brand-image-returns-404-if-no-brand-image-has-been-uploaded-permissionsn
      x-api-path-slug: brandimage-get
      responses:
        200:
          description: OK
      tags:
      - Brand
      - Image
    post:
      summary: Upload brand image
      description: |-
        Uploads a brand image.
        ##### Permissions
        Must have `manage_system` permission.
      operationId: uploads-a-brand-image-permissionsmust-have-manage-system-permission
      x-api-path-slug: brandimage-post
      parameters:
      - in: formData
        name: image
        description: The image to be uploaded
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Brand
      - Image