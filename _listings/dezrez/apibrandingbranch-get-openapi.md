---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Gets a sumary all of the brands for a branch
  version: 1.0.0
  description: Gets a sumary all of the brands for a branch.
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
  /api/role/{id}/savebrandportalexclusions:
    post:
      summary: Get all brands with details for an agency
      description: Get all brands with details for an agency.
      operationId: Role_SaveBrandPortalExclusionsByidBybrandsToSave
      x-api-path-slug: apiroleidsavebrandportalexclusions-post
      parameters:
      - in: body
        name: brandsToSave
        schema:
          $ref: '#/definitions/holder'
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
  /api/agency/portalconfigurations:
    get:
      summary: Get a list of portal configurations for the brand within a branch.
      description: Get a list of portal configurations for the brand within a branch..
      operationId: Agency_PortalConfigurationsBypageSizeBypageNumber
      x-api-path-slug: apiagencyportalconfigurations-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Portal
      - Configurationsthe
      - Brand
      - Within
      - Branch
  /api/agency/updateportalcustomisation:
    put:
      summary: "THIS IS A TEMPORARY ENDPOINT TO Update a portal customisation against
        a brand within a branch.\r\nPLEASE NOTE: This will be replaced by a FE Tool
        in future. If not, Security must be improved."
      description: "This is a temporary endpoint to update a portal customisation
        against a brand within a branch.\r\nplease note: this will be replaced by
        a fe tool in future. if not, security must be improved.."
      operationId: Agency_UpdatePortalCustomisationByportalCustomisation
      x-api-path-slug: apiagencyupdateportalcustomisation-put
      parameters:
      - in: body
        name: portalCustomisation
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - THIS
      - IS
      - TEMPORARY
      - ENDPOINT
      - TO
      - ""
      - Portal
      - Customisation
      - Against
      - Brand
      - Within
      - Branch
      - PLEASE
      - 'NOTE:'
      - This
      - Will
      - Be
      - Replaced
      - By
      - FE
      - Tool
      - In
      - Future
      - ""
      - If
      - Not
      - ""
      - Security
      - Must
      - Be
      - Improved
  /api/agency/{id}/getbrand:
    get:
      summary: Get a specific brand by brandId or default agency brand if brandId
        is not supplied.
      description: Get a specific brand by brandid or default agency brand if brandid
        is not supplied..
      operationId: Agency_GetAgencyBrandByidBybrandId
      x-api-path-slug: apiagencyidgetbrand-get
      parameters:
      - in: query
        name: brandId
        description: The id of brand to get
      - in: path
        name: id
        description: The id of an agency
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Specific
      - Brand
      - By
      - BrandId
      - Default
      - Agency
      - Brand
      - If
      - BrandId
      - Is
      - Not
      - Supplied
  /api/branch/{id}/getbrand:
    get:
      summary: Get a specific brand by brandId or default brand within a branch if
        brandId is not supplied.
      description: Get a specific brand by brandid or default brand within a branch
        if brandid is not supplied..
      operationId: Branch_GetBranchBrandByidBybrandId
      x-api-path-slug: apibranchidgetbrand-get
      parameters:
      - in: query
        name: brandId
        description: The id of brand to get
      - in: path
        name: id
        description: The id of a branch
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Specific
      - Brand
      - By
      - BrandId
      - Default
      - Brand
      - Within
      - Branch
      - If
      - BrandId
      - Is
      - Not
      - Supplied
  /api/branding/{id}/attachexternaldocument:
    put:
      summary: Attaches an external document to brand.
      description: Attaches an external document to brand..
      operationId: Branding_AttachExternalDocumentByidByexternalDocument
      x-api-path-slug: apibrandingidattachexternaldocument-put
      parameters:
      - in: body
        name: externalDocument
        description: Details of the external document
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The BrandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - External
      - Document
      - To
      - Brand
  /api/branding/{id}/uploadandattachdocument:
    put:
      summary: Uploads and attaches a document to a brand.
      description: Uploads and attaches a document to a brand..
      operationId: Branding_UploadAndAttachDocumentByidBydocumentDetails
      x-api-path-slug: apibrandingiduploadandattachdocument-put
      parameters:
      - in: body
        name: documentDetails
        description: Details of the file
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The brandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - Attaches
      - Document
      - To
      - Brand
  /api/branding/{id}/uploadandattachdocumenttodefault:
    put:
      summary: Uploads and attaches a document to a brand.
      description: Uploads and attaches a document to a brand..
      operationId: Branding_UploadAndAttachDocumentToDefaultBrandBydocumentDetailsByid
      x-api-path-slug: apibrandingiduploadandattachdocumenttodefault-put
      parameters:
      - in: body
        name: documentDetails
        description: Details of the file
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - Attaches
      - Document
      - To
      - Brand
  /api/branding/{id}/attachdocument:
    put:
      summary: Attaches a document to a brand.
      description: Attaches a document to a brand..
      operationId: Branding_AttachDocumentByidBydocumentId
      x-api-path-slug: apibrandingidattachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The documentId
      - in: path
        name: id
        description: The BrandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Document
      - To
      - Brand
  /api/branding/{id}/detachdocument:
    put:
      summary: Detaches a document from a brand.
      description: Detaches a document from a brand..
      operationId: Branding_DetachDocumentByidBydocumentId
      x-api-path-slug: apibrandingiddetachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The documentId
      - in: path
        name: id
        description: The BrandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Brand
  /api/branding/{id}/uploaddocumentcustomisation:
    put:
      summary: Upload the data to customise a Brand Document.
      description: Upload the data to customise a brand document..
      operationId: Branding_UploadDocumentCustomisationByidBycustomisationSaveData
      x-api-path-slug: apibrandingiduploaddocumentcustomisation-put
      parameters:
      - in: body
        name: customisationSaveData
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: BrandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Data
      - To
      - Customise
      - Brand
      - Document
  /api/branding/uploadsmstemplate:
    post:
      summary: Upload the data to create a SMS Document Template for a Brand.
      description: Upload the data to create a sms document template for a brand..
      operationId: Branding_UploadSMSTemplateBybrandTemplateSaveDataContract
      x-api-path-slug: apibrandinguploadsmstemplate-post
      parameters:
      - in: body
        name: brandTemplateSaveDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Data
      - To
      - Create
      - SMS
      - Document
      - Templatea
      - Brand
  /api/branding/uploademailtemplate:
    post:
      summary: Upload the data to create a Email Document Template for a Brand.
      description: Upload the data to create a email document template for a brand..
      operationId: Branding_UploadEmailTemplateBybrandTemplateSaveDataContract
      x-api-path-slug: apibrandinguploademailtemplate-post
      parameters:
      - in: body
        name: brandTemplateSaveDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Data
      - To
      - Create
      - Email
      - Document
      - Templatea
      - Brand
  /api/branding/htmladvert/{brandId}:
    post:
      summary: Upload the a html advert for a brand.
      description: Upload the a html advert for a brand..
      operationId: Branding_UpdateHtmlAdvertBybrandIdBybrandHtmlAdvertDataContract
      x-api-path-slug: apibrandinghtmladvertbrandid-post
      parameters:
      - in: body
        name: brandHtmlAdvertDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: brandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Html
      - Adverta
      - Brand
  /api/branding/htmladverts/{brandId}:
    get:
      summary: Upload the a html advert for a brand.
      description: Upload the a html advert for a brand..
      operationId: Branding_HtmlAdvertsBybrandId
      x-api-path-slug: apibrandinghtmladvertsbrandid-get
      parameters:
      - in: path
        name: brandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Html
      - Adverta
      - Brand
  /api/documentgeneration/headertemplates:
    get:
      summary: Returns a list of header templates associated to this agency with their
        associated brand info
      description: Returns a list of header templates associated to this agency with
        their associated brand info.
      operationId: DocumentGeneration_GetPrintableHeaderTemplates
      x-api-path-slug: apidocumentgenerationheadertemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Header
      - Templates
      - Associated
      - To
      - This
      - Agency
      - Their
      - Associated
      - Brand
      - Info
  /api/branding/branch:
    get:
      summary: Gets a sumary all of the brands for a branch
      description: Gets a sumary all of the brands for a branch.
      operationId: Branding_GetBranch
      x-api-path-slug: apibrandingbranch-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Sumary
      - ""
      - Of
      - Brandsa
      - Branch
  /api/Branding:
    get:
      summary: Gets a sumary all of the brands for a agency
      description: Gets a sumary all of the brands for a agency.
      operationId: Branding_Get
      x-api-path-slug: apibranding-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Sumary
      - ""
      - Of
      - Brandsa
      - Agency
  /api/branch/{id}/Brandings:
    get:
      summary: Get a Branch brandings by its id.
      description: Get a branch brandings by its id..
      operationId: Branch_BrandingsByid
      x-api-path-slug: apibranchidbrandings-get
      parameters:
      - in: path
        name: id
        description: The id of the Branch brandings  to get
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Branch
      - Brandings
      - By
      - Its
      - Id
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