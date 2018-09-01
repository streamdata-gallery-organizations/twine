---
swagger: "2.0"
x-collection-name: Twine
x-complete: 0
info:
  title: Twine Get a calendar event
  description: Get a calendar event by id
  version: 7.18.0
host: api.twinehealth.com
basePath: /pub
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /action:
    post:
      summary: Create action
      description: Create a plan action
      operationId: createAction
      x-api-path-slug: action-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Action
  /action/{id}:
    get:
      summary: Get an action
      description: Get a health action from a patient's plan.
      operationId: fetchAction
      x-api-path-slug: actionid-get
      parameters:
      - in: path
        name: id
        description: Action identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Action
    patch:
      summary: Update an action
      description: Update a health action from a patient's plan.
      operationId: updateAction
      x-api-path-slug: actionid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Action identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Action
  /bundle:
    post:
      summary: Create bundle
      description: Create a bundle in a patient's plan
      operationId: createBundle
      x-api-path-slug: bundle-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Bundle
  /bundle/{id}:
    get:
      summary: Get a bundle
      description: Get a bundle from a patient's plan.
      operationId: fetchBundle
      x-api-path-slug: bundleid-get
      parameters:
      - in: path
        name: id
        description: Bundle identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Bundle
    patch:
      summary: Update a bundle
      description: Updte a bundle from a patient's plan.
      operationId: updateBundle
      x-api-path-slug: bundleid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Bundle identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Bundle
  /calendar_event:
    get:
      summary: List calendar events
      description: Get a list of calendar events
      operationId: fetchCalendarEvents
      x-api-path-slug: calendar-event-get
      parameters:
      - in: query
        name: filter[attendees]
        description: Comma-separated list of coach or patient ids
      - in: query
        name: filter[completed]
        description: If not specified, return all calendar events
      - in: query
        name: filter[completed_at]
        description: The start (inclusive) and end (exclusive) dates are ISO date
          and time strings separated by `
      - in: query
        name: filter[created_at]
        description: The start (inclusive) and end (exclusive) dates are ISO date
          and time strings separated by `
      - in: query
        name: filter[end_at]
        description: The start (inclusive) and end (exclusive) dates are ISO date
          and time strings separated by `
      - in: query
        name: filter[groups]
        description: Comma-separated list of group ids
      - in: query
        name: filter[organization]
        description: Twine organization id
      - in: query
        name: filter[patient]
        description: Patient id to fetch calendar event
      - in: query
        name: filter[start_at]
        description: The start (inclusive) and end (exclusive) dates are ISO date
          and time strings separated by `
      - in: query
        name: filter[type]
        description: Calendar event type
      - in: query
        name: filter[updated_at]
        description: The start (inclusive) and end (exclusive) dates are ISO date
          and time strings separated by `
      - in: query
        name: include
        description: List of related resources to include in the response
      - in: query
        name: page[number]
        description: Page number
      - in: query
        name: page[size]
        description: Page size
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Calendar
      - Events
    post:
      summary: Create calendar event
      description: Create a calendar event for a patient. Attribute `all_day` must
        be set to `true` and `end_at` cannot be set for `plan-check-in` event type.
      operationId: createCalendarEvent
      x-api-path-slug: calendar-event-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Calendar
      - Event
  /calendar_event/{id}:
    delete:
      summary: Delete a calendar event
      description: Delete a calendar event by id
      operationId: deleteCalendarEvent
      x-api-path-slug: calendar-eventid-delete
      parameters:
      - in: path
        name: id
        description: Calendar event identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Calendar
      - Event
    get:
      summary: Get a calendar event
      description: Get a calendar event by id
      operationId: fetchCalendarEvent
      x-api-path-slug: calendar-eventid-get
      parameters:
      - in: path
        name: id
        description: Calendar event identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Calendar
      - Event
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