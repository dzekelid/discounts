---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 1
info:
  title: Eventbrite
  description: the-eventbrite-api-is-the-best-way-to-integrate-and-extend-eventbrite-for-your-event-or-organising-needs-version-3-of-the-api-brings-you-faster-responses-consistent-data-types-more-endpoints-and-easier-debugging-and-testing
  version: 1.0.0
host: www.eventbriteapi.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /discounts/:discount_id/:
    get:
      summary: Get Discounts Discount
      description: Returns the cross_event_discount with the specified :discount_id.
      operationId: getDiscountsDiscount
      x-api-path-slug: discountsdiscount-id-get
      responses:
        200:
          description: OK
      tags:
      - Discounts
      - Discount
    post:
      summary: Add Discounts Discount
      description: Updates the discount with the specified :discount_id. Returns the
        updated cross_event_discount. The fields sent are the ones that are going
        to be updated, the fields that are not sent will be unchanged. The same conditions
        and notes for the discount creation apply.
      operationId: postDiscountsDiscount
      x-api-path-slug: discountsdiscount-id-post
      parameters:
      - in: query
        name: discount.amount_off
        description: Fixed reduction amount
        type: query
      - in: query
        name: discount.code
        description: Code used to activate discount
        type: query
      - in: query
        name: discount.end_date
        description: Allow use until this date
        type: query
      - in: query
        name: discount.end_date_relative
        description: Allow use until this number of seconds before the event starts
        type: query
      - in: query
        name: discount.hold_ids
        description: IDs of holds this discount can unlock
        type: query
      - in: query
        name: discount.percent_off
        description: Percentage reduction
        type: query
      - in: query
        name: discount.quantity_available
        description: Number of discount uses
        type: query
      - in: query
        name: discount.start_date
        description: Allow use from this date
        type: query
      - in: query
        name: discount.start_date_relative
        description: Allow use from this number of seconds before the event starts
        type: query
      - in: query
        name: discount.ticket_class_ids
        description: IDs of tickets to limit discount to
        type: query
      responses:
        200:
          description: OK
      tags:
      - Discounts
      - Discount
    delete:
      summary: Delete Discounts Discount
      description: |-
        Deletes the cross_event_discount with the specified :discount_id.
        Only unused discounts can be deleted.
      operationId: deleteDiscountsDiscount
      x-api-path-slug: discountsdiscount-id-delete
      responses:
        200:
          description: OK
      tags:
      - Discounts
      - Discount
  /discounts/:
    post:
      summary: Add Discounts
      description: Creates a discount. Returns the created cross_event_discount.
      operationId: postDiscounts
      x-api-path-slug: discounts-post
      parameters:
      - in: query
        name: discount.amount_off
        description: Fixed reduction amount
        type: query
      - in: query
        name: discount.code
        description: Code used to activate discount
        type: query
      - in: query
        name: discount.end_date
        description: Allow use until this date
        type: query
      - in: query
        name: discount.end_date_relative
        description: Allow use until this number of seconds before the event starts
        type: query
      - in: query
        name: discount.event_id
        description: ID of the event
        type: query
      - in: query
        name: discount.hold_ids
        description: IDs of holds this discount can unlock
        type: query
      - in: query
        name: discount.percent_off
        description: Percentage reduction
        type: query
      - in: query
        name: discount.quantity_available
        description: Number of discount uses
        type: query
      - in: query
        name: discount.start_date
        description: Allow use from this date
        type: query
      - in: query
        name: discount.start_date_relative
        description: Allow use from this number of seconds before the event starts
        type: query
      - in: query
        name: discount.ticket_class_ids
        description: IDs of tickets to limit discount to
        type: query
      - in: query
        name: discount.ticket_group_id
        description: ID of the ticket group
        type: query
      - in: query
        name: discount.type
        description: The type of discount
        type: query
      responses:
        200:
          description: OK
      tags:
      - Discounts
  /events/{id}/discounts/:
    get:
      summary: Get Events  Discounts
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/users/#ebapi-get-users-user-id-discounts
      operationId: getEventsDiscounts
      x-api-path-slug: eventsiddiscounts-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - ""
      - Discounts
    post:
      summary: Add Events  Discounts
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts
      operationId: postEventsDiscounts
      x-api-path-slug: eventsiddiscounts-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - ""
      - Discounts
  /events/{id}/discounts/:discount_id/:
    get:
      summary: Get Events  Discounts Discount
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id
      operationId: getEventsDiscountsDiscount
      x-api-path-slug: eventsiddiscountsdiscount-id-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - ""
      - Discounts
      - Discount
    post:
      summary: Add Events  Discounts Discount
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts-discount-id
      operationId: postEventsDiscountsDiscount
      x-api-path-slug: eventsiddiscountsdiscount-id-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - ""
      - Discounts
      - Discount
    delete:
      summary: Delete Events  Discounts Discount
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-delete-discounts-discount-id
      operationId: deleteEventsDiscountsDiscount
      x-api-path-slug: eventsiddiscountsdiscount-id-delete
      responses:
        200:
          description: OK
      tags:
      - Events
      - ""
      - Discounts
      - Discount
  /events/{id}/public_discounts/:
    get:
      summary: Get Events  Public Discounts
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/users/#ebapi-get-users-user-id-discounts
      operationId: getEventsPublicDiscounts
      x-api-path-slug: eventsidpublic-discounts-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - ""
      - Public
      - Discounts
    post:
      summary: Add Events  Public Discounts
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts
      operationId: postEventsPublicDiscounts
      x-api-path-slug: eventsidpublic-discounts-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - ""
      - Public
      - Discounts
  /events/{id}/public_discounts/:discount_id/:
    get:
      summary: Get Events  Public Discounts Discount
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id
      operationId: getEventsPublicDiscountsDiscount
      x-api-path-slug: eventsidpublic-discountsdiscount-id-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - ""
      - Public
      - Discounts
      - Discount
    post:
      summary: Add Events  Public Discounts Discount
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts-discount-id
      operationId: postEventsPublicDiscountsDiscount
      x-api-path-slug: eventsidpublic-discountsdiscount-id-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - ""
      - Public
      - Discounts
      - Discount
    delete:
      summary: Delete Events  Public Discounts Discount
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-delete-discounts-discount-id
      operationId: deleteEventsPublicDiscountsDiscount
      x-api-path-slug: eventsidpublic-discountsdiscount-id-delete
      responses:
        200:
          description: OK
      tags:
      - Events
      - ""
      - Public
      - Discounts
      - Discount
  /users/:user_id/discounts/:
    get:
      summary: Get Users User  Discounts
      description: |-
        Returns a paginated response of cross_event_discount for the specified user.
        This operation is only supported for the currently authenticated user. The alias me (/users/me/) may be used.
      operationId: getUsersUserDiscounts
      x-api-path-slug: usersuser-iddiscounts-get
      parameters:
      - in: query
        name: code
        description: Search term to find discounts by code/name, in an exact match
          behavior
        type: query
      - in: query
        name: code_filter
        description: Search term to filter discounts by name
        type: query
      - in: query
        name: event_id
        description: ID of the event
        type: query
      - in: query
        name: order_by
        description: 'How to order the results (Valid choices are: code_asc, code_desc,
          discount_type_asc, discount_type_desc, start_asc, or start_desc)'
        type: query
      - in: query
        name: page_size
        description: Number of records in each page
        type: query
      - in: query
        name: scope
        description: Type of discount scopes
        type: query
      - in: query
        name: ticket_group_id
        description: ID of the ticket group
        type: query
      - in: query
        name: type
        description: Filter discounts with a specific discount type set
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - ""
      - Discounts
---