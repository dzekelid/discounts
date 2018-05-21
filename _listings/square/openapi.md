---
swagger: "2.0"
x-collection-name: Square
x-complete: 1
info:
  title: Square Connect API
  description: client-library-for-accessing-the-square-connect-apis
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: 1.0.0
host: connect.squareup.com
basePath: v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{location_id}/discounts:
    post:
      summary: Post Location Discounts
      description: Post location discounts.
      operationId: postLocationDiscounts
      x-api-path-slug: location-iddiscounts-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the location to create an item for
      responses:
        200:
          description: OK
      tags:
      - Location
      - Discounts
    get:
      summary: Get Location Discounts
      description: Lists all of a location's discounts.
      operationId: getLocationDiscounts
      x-api-path-slug: location-iddiscounts-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the location to list categories for
      responses:
        200:
          description: OK
      tags:
      - Location
      - Discounts
  /{location_id}/discounts/{discount_id}:
    put:
      summary: Put Location Discounts Discount
      description: Modifies the details of an existing discount.
      operationId: putLocationDiscountsDiscount
      x-api-path-slug: location-iddiscountsdiscount-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: discount_id
        description: The ID of the discount to edit
      - in: path
        name: location_id
        description: The ID of the categorys associated location
      responses:
        200:
          description: OK
      tags:
      - Location
      - Discounts
    delete:
      summary: Delete Location Discounts Discount
      description: Delete location discounts discount.
      operationId: deleteLocationDiscountsDiscount
      x-api-path-slug: location-iddiscountsdiscount-id-delete
      parameters:
      - in: path
        name: discount_id
        description: The ID of the discount to delete
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - Location
      - Discounts
---