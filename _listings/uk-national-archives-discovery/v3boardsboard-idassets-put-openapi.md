---
swagger: "2.0"
x-collection-name: UK National Archives Discovery
x-complete: 0
info:
  title: Getty Images Search API Put Boards Board Assets
  description: <b>***beta***</b> add assets to a board.
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