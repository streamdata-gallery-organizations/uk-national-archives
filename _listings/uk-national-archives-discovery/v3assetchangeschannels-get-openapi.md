---
swagger: "2.0"
x-collection-name: UK National Archives Discovery
x-complete: 0
info:
  title: Getty Images Search API Get Asset Changes Channels
  description: Retrieves the channel data for the partner. this data can be used to
    populate the channel_id parameter in the put asset changes query..
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