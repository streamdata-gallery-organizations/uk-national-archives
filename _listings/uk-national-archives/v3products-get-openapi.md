---
swagger: "2.0"
x-collection-name: UK National Archives
x-complete: 0
info:
  title: Getty Images Search API Get Products
  description: Get products.
  version: "3.0"
host: api.gettyimages.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/asset-changes/change-sets:
    put:
      summary: Put Asset Changes Change Sets
      description: Generates asset changes..
      operationId: putV3AssetChangesChangeSets
      x-api-path-slug: v3assetchangeschangesets-put
      parameters:
      - in: header
        name: Accept-Language
        description: Accept-Language parameter optional
      - in: header
        name: Authorization
        description: Authorization token required
      - in: query
        name: batch_size
        description: Specifies the number of assets to return
      - in: query
        name: channel_id
        description: Specifies the id of the channel for the asset data
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Changes
      - Change
      - Sets
  /v3/asset-changes/change-sets/{change-set-id}:
    delete:
      summary: Delete Asset Changes Change Sets Change Set
      description: Confirm asset changes acknowledges receipt of asset changes..
      operationId: deleteV3AssetChangesChangeSetsChangeSet
      x-api-path-slug: v3assetchangeschangesetschangesetid-delete
      parameters:
      - in: header
        name: Accept-Language
        description: Accept-Language parameter optional
      - in: header
        name: Authorization
        description: Authorization token required
      - in: path
        name: change-set-id
        description: Specify the change-set-id associated with a transaction resource
          whose receipt you want to confirm
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Changes
      - Change
      - Sets
      - Change
      - Set
  /v3/asset-changes/channels:
    get:
      summary: Get Asset Changes Channels
      description: Retrieves the channel data for the partner. this data can be used
        to populate the channel_id parameter in the put asset changes query..
      operationId: getV3AssetChangesChannels
      x-api-path-slug: v3assetchangeschannels-get
      parameters:
      - in: header
        name: Accept-Language
        description: Accept-Language parameter optional
      - in: header
        name: Authorization
        description: Authorization token required
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Changes
      - Channels
  /v3/asset-registrations:
    post:
      summary: Post Asset Registrations
      description: Register a list of customer assets..
      operationId: postV3AssetRegistrations
      x-api-path-slug: v3assetregistrations-post
      parameters:
      - in: header
        name: Accept-Language
        description: Accept-Language parameter optional
      - in: header
        name: Authorization
        description: Authorization token required
      - in: body
        name: request
        description: Specify JSON containing an array of asset ids to register
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Registrations
  /v3/boards:
    get:
      summary: Get Boards
      description: <b>***beta***</b> get all boards that the user participates in.
      operationId: getV3Boards
      x-api-path-slug: v3boards-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: board_relationship
        description: Search for boards the user owns or has been invited to as an
          editor
      - in: query
        name: page
        description: Request results starting at a page number (default is 1)
      - in: query
        name: page_size
        description: Request number of boards to return in each page
      - in: query
        name: sort_order
        description: Sort the list of boards by last update date or name
      responses:
        200:
          description: OK
      tags:
      - Boards
    post:
      summary: Post Boards
      description: <b>***beta***</b> create a new board.
      operationId: postV3Boards
      x-api-path-slug: v3boards-post
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: body
        name: new_board
        description: Specify a name and description of the board to create (name is
          required)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Boards
  /v3/boards/{board_id}:
    delete:
      summary: Delete Boards Board
      description: <b>***beta***</b> delete a board.
      operationId: deleteV3BoardsBoard
      x-api-path-slug: v3boardsboard-id-delete
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
        description: Specify the board to delete
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Board
    get:
      summary: Get Boards Board
      description: <b>***beta***</b> get assets and metadata for a specific board.
      operationId: getV3BoardsBoard
      x-api-path-slug: v3boardsboard-id-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
        description: Retrieve details for a specific board
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Board
    put:
      summary: Put Boards Board
      description: <b>***beta***</b> update a board.
      operationId: putV3BoardsBoard
      x-api-path-slug: v3boardsboard-id-put
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
        description: Specify the board to update
      - in: body
        name: board_info
        description: Specify a new name and description for the board (name is required)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Board
  /v3/boards/{board_id}/assets:
    delete:
      summary: Delete Boards Board Assets
      description: <b>***beta***</b> remove assets from a board.
      operationId: deleteV3BoardsBoardAssets
      x-api-path-slug: v3boardsboard-idassets-delete
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: query
        name: asset_ids
        description: List the assets to be removed from the board
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
        description: Specify the board to remove assets from
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Board
      - Assets
    put:
      summary: Put Boards Board Assets
      description: <b>***beta***</b> add assets to a board.
      operationId: putV3BoardsBoardAssets
      x-api-path-slug: v3boardsboard-idassets-put
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: body
        name: board_assets
        description: List assets to add to the board
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: board_id
        description: Specify the board to add assets to
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Board
      - Assets
  /v3/boards/{board_id}/assets/{asset_id}:
    delete:
      summary: Delete Boards Board Assets Asset
      description: <b>***beta***</b> remove an asset from a board.
      operationId: deleteV3BoardsBoardAssetsAsset
      x-api-path-slug: v3boardsboard-idassetsasset-id-delete
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: path
        name: asset_id
        description: Specify the asset to remove from the board
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
        description: Specify the board to remove an asset from
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Board
      - Assets
      - Asset
    put:
      summary: Put Boards Board Assets Asset
      description: <b>***beta***</b> add an asset to a board.
      operationId: putV3BoardsBoardAssetsAsset
      x-api-path-slug: v3boardsboard-idassetsasset-id-put
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: path
        name: asset_id
        description: Specify the asset to add to the board
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
        description: Specify the board to add an asset to
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Board
      - Assets
      - Asset
  /v3/boards/{board_id}/comments:
    get:
      summary: Get Boards Board Comments
      description: <b>***beta***</b> get comments from a board.
      operationId: getV3BoardsBoardComments
      x-api-path-slug: v3boardsboard-idcomments-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
        description: Specify the board to retrieve comments from
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Board
      - Comments
    post:
      summary: Post Boards Board Comments
      description: <b>***beta***</b> add a comment to a board.
      operationId: postV3BoardsBoardComments
      x-api-path-slug: v3boardsboard-idcomments-post
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
        description: Specify the board to add a comment to
      - in: body
        name: comment
        description: Comment to be added to the board
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Board
      - Comments
  /v3/boards/{board_id}/comments/{comment_id}:
    delete:
      summary: Delete Boards Board Comments Comment
      description: <b>***beta***</b> delete a comment from a board.
      operationId: deleteV3BoardsBoardCommentsComment
      x-api-path-slug: v3boardsboard-idcommentscomment-id-delete
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
        description: Specify the board containing the comment to delete
      - in: path
        name: comment_id
        description: Specify the comment to delete
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Board
      - Comments
      - Comment
  /v3/collections:
    get:
      summary: Get Collections
      description: Gets collections applicable for the customer..
      operationId: getV3Collections
      x-api-path-slug: v3collections-get
      parameters:
      - in: header
        name: Accept-Language
        description: Specifies the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      responses:
        200:
          description: OK
      tags:
      - Collections
  /v3/countries:
    get:
      summary: Get Countries
      description: Gets countries codes and names..
      operationId: getV3Countries
      x-api-path-slug: v3countries-get
      parameters:
      - in: header
        name: Accept-Language
        description: Specifies the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      responses:
        200:
          description: OK
      tags:
      - Countries
  /v3/downloads:
    get:
      summary: Get Downloads
      description: Returns information about a customer's downloaded assets..
      operationId: getV3Downloads
      x-api-path-slug: v3downloads-get
      parameters:
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: company_downloads
        description: If specified, returns the list of previously downloaded images
          for all users in your company
      - in: query
        name: date_from
        description: If specified, select assets downloaded on or after this date
      - in: query
        name: date_to
        description: If specified, select assets downloaded on or before this date
      - in: query
        name: page
        description: Identifies page to return
      - in: query
        name: page_size
        description: Specifies page size
      - in: query
        name: product_type
        description: Specifies product type to be included in the previous download
          results
      responses:
        200:
          description: OK
      tags:
      - Downloads
  /v3/downloads/images/{id}:
    post:
      summary: Post Downloads Images
      description: Download an image.
      operationId: postV3DownloadsImages
      x-api-path-slug: v3downloadsimagesid-post
      parameters:
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: auto_download
        description: Specifies whether to auto-download the image
      - in: body
        name: download_details
        description: Additional information required from specific customers when
          downloading
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: file_type
        description: File Type expressed with three character file extension
      - in: query
        name: height
        description: Specifies the pixel height of the particular image to download
      - in: path
        name: id
        description: Id of image to download
      - in: query
        name: product_id
        description: Identifier of the instance for the selected product offering
          type
      - in: query
        name: product_type
        description: Product type
      responses:
        200:
          description: OK
      tags:
      - Downloads
      - Images
  /v3/downloads/videos/{id}:
    post:
      summary: Post Downloads Veos
      description: Download a video.
      operationId: postV3DownloadsVeos
      x-api-path-slug: v3downloadsvideosid-post
      parameters:
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: auto_download
        description: Specifies whether to auto-download the video
      - in: path
        name: id
        description: Id of video to download
      - in: query
        name: product_id
        description: Identifier of the instance for the selected product offering
          type
      - in: query
        name: size
        description: Specifies the size to be downloaded
      responses:
        200:
          description: OK
      tags:
      - Downloads
      - Veos
  /v3/downloads/{id}:
    post:
      summary: Post Downloads
      description: Download an image.
      operationId: postV3Downloads
      x-api-path-slug: v3downloadsid-post
      parameters:
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: auto_download
        description: Specifies whether to auto-download the image
      - in: body
        name: download_details
        description: Additional information required from specific customers when
          downloading
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: file_type
        description: File Type expressed with three character file extension
      - in: query
        name: height
        description: Specifies the pixel height of the particular image to download
      - in: path
        name: id
        description: Id of image to download
      - in: query
        name: product_id
        description: Identifier of the instance for the selected product offering
          type
      - in: query
        name: product_type
        description: Product type
      responses:
        200:
          description: OK
      tags:
      - Downloads
  /v3/events:
    get:
      summary: Get Events
      description: Get metadata for multiple events.
      operationId: getV3Events
      x-api-path-slug: v3events-get
      parameters:
      - in: header
        name: Accept-Language
        description: Specifies the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: A comma separated list of fields to return in the response
      - in: query
        name: ids
        description: A comma separated list of event ids
      responses:
        200:
          description: OK
      tags:
      - Events
  /v3/events/{id}:
    get:
      summary: Get Events
      description: Get metadata for a single event.
      operationId: getV3Events
      x-api-path-slug: v3eventsid-get
      parameters:
      - in: header
        name: Accept-Language
        description: Specifies the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: A comma separated list of fields to return in the response
      - in: path
        name: id
        description: An event id
      responses:
        200:
          description: OK
      tags:
      - Events
  /v3/images:
    get:
      summary: Get Images
      description: Get metadata for multiple images by supplying multiple image ids.
      operationId: getV3Images
      x-api-path-slug: v3images-get
      parameters:
      - in: header
        name: Accept-Language
        description: Specifies the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: Specifies fields to return
      - in: query
        name: ids
        description: Specifies one or more image ids to return
      responses:
        200:
          description: OK
      tags:
      - Images
  /v3/images/{id}:
    get:
      summary: Get Images
      description: Get metadata for a single image by supplying one image id.
      operationId: getV3Images
      x-api-path-slug: v3imagesid-get
      parameters:
      - in: header
        name: Accept-Language
        description: Specifies the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: Specifies fields to return
      - in: path
        name: id
        description: An image id
      responses:
        200:
          description: OK
      tags:
      - Images
  /v3/images/{id}/similar:
    get:
      summary: Get Images Similar
      description: Search for images similar to an image.
      operationId: getV3ImagesSimilar
      x-api-path-slug: v3imagesidsimilar-get
      parameters:
      - in: header
        name: Accept-Language
        description: Specifies the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: Specifies fields to return
      - in: path
        name: id
        description: Identifies an existing image
      - in: query
        name: page
        description: Identifies page to return
      - in: query
        name: page_size
        description: Specifies page size
      responses:
        200:
          description: OK
      tags:
      - Images
      - Similar
  /v3/products:
    get:
      summary: Get Products
      description: Get products.
      operationId: getV3Products
      x-api-path-slug: v3products-get
      parameters:
      - in: header
        name: Accept-Language
        description: Specifies the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: Comma separated list of fields
      responses:
        200:
          description: OK
      tags:
      - Products
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