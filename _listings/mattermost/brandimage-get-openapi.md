---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Get brand image
  description: |-
    Get the previously uploaded brand image. Returns 404 if no brand image has been uploaded.
    ##### Permissions
    No permission required.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
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