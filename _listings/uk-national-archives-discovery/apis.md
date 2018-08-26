---
name: UK National Archives Discovery
x-slug: uk-national-archives-discovery
description: ""
image: ""
x-kinRank: "7"
x-alexaRank: "0"
tags: UK National Archives Discovery
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/apis.md
specificationVersion: "0.14"
apis:
- name: Getty Images Search API Put Asset Changes Change Sets
  x-api-slug: getty-images-search-api
  description: Generates asset changes..
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/asset-changes/change-sets
  tags: Asset,Changes,Change,Sets
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3assetchangeschangesets-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3assetchangeschangesets-put-openapi.md
- name: Getty Images Search API Delete Asset Changes Change Sets Change Set
  x-api-slug: getty-images-search-api
  description: Confirm asset changes acknowledges receipt of asset changes..
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/asset-changes/change-sets/{change-set-id}
  tags: Asset,Changes,Change,Sets,Change,Set
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3assetchangeschangesetschangesetid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3assetchangeschangesetschangesetid-delete-openapi.md
- name: Getty Images Search API Get Asset Changes Channels
  x-api-slug: getty-images-search-api
  description: Retrieves the channel data for the partner. this data can be used to
    populate the channel_id parameter in the put asset changes query..
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/asset-changes/channels
  tags: Asset,Changes,Channels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3assetchangeschannels-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3assetchangeschannels-get-openapi.md
- name: Getty Images Search API Post Asset Registrations
  x-api-slug: getty-images-search-api
  description: Register a list of customer assets..
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/asset-registrations
  tags: Asset,Registrations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3assetregistrations-post-openapi.md
- name: Getty Images Search API Get Boards
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> get all boards that the user participates in.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards
  tags: Boards
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3boards-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3boards-get-openapi.md
- name: Getty Images Search API Post Boards
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> create a new board.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards
  tags: Boards
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3boards-post-openapi.md
- name: Getty Images Search API Delete Boards Board
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> delete a board.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}
  tags: Boards,Board
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3boardsboard-id-delete-openapi.md
- name: Getty Images Search API Get Boards Board
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> get assets and metadata for a specific board.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}
  tags: Boards,Board
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3boardsboard-id-get-openapi.md
- name: Getty Images Search API Put Boards Board
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> update a board.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}
  tags: Boards,Board
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3boardsboard-id-put-openapi.md
- name: Getty Images Search API Delete Boards Board Assets
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> remove assets from a board.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/assets
  tags: Boards,Board,Assets
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3boardsboard-idassets-delete-openapi.md
- name: Getty Images Search API Put Boards Board Assets
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> add assets to a board.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/assets
  tags: Boards,Board,Assets
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3boardsboard-idassets-put-openapi.md
- name: Getty Images Search API Delete Boards Board Assets Asset
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> remove an asset from a board.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/assets/{asset_id}
  tags: Boards,Board,Assets,Asset
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3boardsboard-idassetsasset-id-delete-openapi.md
- name: Getty Images Search API Put Boards Board Assets Asset
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> add an asset to a board.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/assets/{asset_id}
  tags: Boards,Board,Assets,Asset
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3boardsboard-idassetsasset-id-put-openapi.md
- name: Getty Images Search API Get Boards Board Comments
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> get comments from a board.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/comments
  tags: Boards,Board,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3boardsboard-idcomments-get-openapi.md
- name: Getty Images Search API Post Boards Board Comments
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> add a comment to a board.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/comments
  tags: Boards,Board,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3boardsboard-idcomments-post-openapi.md
- name: Getty Images Search API Delete Boards Board Comments Comment
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> delete a comment from a board.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/comments/{comment_id}
  tags: Boards,Board,Comments,Comment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3boardsboard-idcommentscomment-id-delete-openapi.md
- name: Getty Images Search API Get Collections
  x-api-slug: getty-images-search-api
  description: Gets collections applicable for the customer..
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/collections
  tags: Collections
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3collections-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3collections-get-openapi.md
- name: Getty Images Search API Get Countries
  x-api-slug: getty-images-search-api
  description: Gets countries codes and names..
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/countries
  tags: Countries
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3countries-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3countries-get-openapi.md
- name: Getty Images Search API Get Downloads
  x-api-slug: getty-images-search-api
  description: Returns information about a customer's downloaded assets..
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/downloads
  tags: Downloads
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3downloads-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3downloads-get-openapi.md
- name: Getty Images Search API Post Downloads Images
  x-api-slug: getty-images-search-api
  description: Download an image.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/downloads/images/{id}
  tags: Downloads,Images
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3downloadsimagesid-post-openapi.md
- name: Getty Images Search API Post Downloads Veos
  x-api-slug: getty-images-search-api
  description: Download a video.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/downloads/videos/{id}
  tags: Downloads,Veos
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3downloadsvideosid-post-openapi.md
- name: Getty Images Search API Post Downloads
  x-api-slug: getty-images-search-api
  description: Download an image.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/downloads/{id}
  tags: Downloads
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3downloadsid-post-openapi.md
- name: Getty Images Search API Get Events
  x-api-slug: getty-images-search-api
  description: Get metadata for multiple events.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/events
  tags: Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3events-get-openapi.md
- name: Getty Images Search API Get Events
  x-api-slug: getty-images-search-api
  description: Get metadata for a single event.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/events/{id}
  tags: Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3eventsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3eventsid-get-openapi.md
- name: Getty Images Search API Get Images
  x-api-slug: getty-images-search-api
  description: Get metadata for multiple images by supplying multiple image ids.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/images
  tags: Images
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3images-get-openapi.md
- name: Getty Images Search API Get Images
  x-api-slug: getty-images-search-api
  description: Get metadata for a single image by supplying one image id.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/images/{id}
  tags: Images
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3imagesid-get-openapi.md
- name: Getty Images Search API Get Images Similar
  x-api-slug: getty-images-search-api
  description: Search for images similar to an image.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/images/{id}/similar
  tags: Images,Similar
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3imagesidsimilar-get-openapi.md
- name: Getty Images Search API Get Products
  x-api-slug: getty-images-search-api
  description: Get products.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/products
  tags: Products
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3products-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3products-get-openapi.md
- name: Getty Images Search API Get Purchased Assets
  x-api-slug: getty-images-search-api
  description: Get previously purchased images and video.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/purchased-assets
  tags: Purchased,Assets
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3purchasedassets-get-openapi.md
- name: Getty Images Search API Get Purchased Images
  x-api-slug: getty-images-search-api
  description: Get previously purchased images.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/purchased-images
  tags: Purchased,Images
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3purchasedimages-get-openapi.md
- name: Getty Images Search API Get Search Events
  x-api-slug: getty-images-search-api
  description: Search for events.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/search/events
  tags: Search,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3searchevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3searchevents-get-openapi.md
- name: Getty Images Search API Get Search Images
  x-api-slug: getty-images-search-api
  description: Search for both creative and editorial images.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/search/images
  tags: Search,Images
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3searchimages-get-openapi.md
- name: Getty Images Search API Get Search Images Creative
  x-api-slug: getty-images-search-api
  description: Search for creative images only.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/search/images/creative
  tags: Search,Images,Creative
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3searchimagescreative-get-openapi.md
- name: Getty Images Search API Get Search Images Editorial
  x-api-slug: getty-images-search-api
  description: Search for editorial images only.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/search/images/editorial
  tags: Search,Images,Editorial
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3searchimageseditorial-get-openapi.md
- name: Getty Images Search API Get Search Veos
  x-api-slug: getty-images-search-api
  description: Search for both creative and editorial videos.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/search/videos
  tags: Search,Veos
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3searchvideos-get-openapi.md
- name: Getty Images Search API Get Search Veos Creative
  x-api-slug: getty-images-search-api
  description: Search for creative videos.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/search/videos/creative
  tags: Search,Veos,Creative
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3searchvideoscreative-get-openapi.md
- name: Getty Images Search API Get Search Veos Editorial
  x-api-slug: getty-images-search-api
  description: Search for editorial videos.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/search/videos/editorial
  tags: Search,Veos,Editorial
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3searchvideoseditorial-get-openapi.md
- name: Getty Images Search API Put Usage Batches
  x-api-slug: getty-images-search-api
  description: Report usage of assets via a batch format..
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/usage-batches/{id}
  tags: Usage,Batches
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3usagebatchesid-put-openapi.md
- name: Getty Images Search API Get Veos
  x-api-slug: getty-images-search-api
  description: Get metadata for multiple videos by supplying multiple video ids.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/videos
  tags: Veos
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3videos-get-openapi.md
- name: Getty Images Search API Get Veos
  x-api-slug: getty-images-search-api
  description: Get metadata for a single video by supplying one video id.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/videos/{id}
  tags: Veos
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/v3videosid-get-openapi.md
- name: Getty Images Search API
  x-api-slug: getty-images-search-api
  description: Our set of APIs enable seamless integration of Getty Images expansive
    content, powerful search and rich metadata directly into your internal workflows,
    products and services. With Connects API solutions, you can fully control, customize
    and scale as you grow.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com//
  tags: UK National Archives Discovery
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/uk-national-archives-discovery/master/_listings/uk-national-archives-discovery/openapi.md
x-common:
- type: x-website
  url: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
- type: x-website
  url: http:///Search
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---