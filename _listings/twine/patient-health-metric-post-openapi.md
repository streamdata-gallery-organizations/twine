---
swagger: "2.0"
x-collection-name: Twine
x-complete: 0
info:
  title: Twine Create patient health metrics
  description: |-
    Create one or more patient health metrics.

    Example for creating a patient health result with a patient specified using `meta.query` instead of `id`:

    ```JSON
      {
        "data": {
          "type": "patient_health_metric",
           "attributes": {
             "code": {
               "system": "LOINC",
               "value": "13457-7"
             },
             "type": "ldl_cholesterol",
             "occurred_at": "2017-03-14T11:00:57.000Z",
             "value": "121",
             "unit": "mg/dl"
          },
          "relationships": {
            "patient": {
              "data": {
                "type": "patient",
                "meta": {
                  "query": {
                    "identifier": {
                      "system": "medical-record-number",
                      "value": "121212"
                    },
                    "organization": "58c4554710123c5c40dbab81"
                  }
                }
              }
            }
          }
        }
      }
    ```
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
    patch:
      summary: Update a calendar event
      description: Update a calendar event for a patient. Attribute `all_day` must
        be true and `end_at` cannot be specified for `plan-check-in` event type. To
        mark a calendar event as 'completed', set `completed_at` and `completed_by`
        to desired values.  To mark a completed calendar event as 'not completed',
        set `completed_at` and `completed_by` to `null`.
      operationId: updateCalendarEvent
      x-api-path-slug: calendar-eventid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
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
  /coach/{id}:
    get:
      summary: Get a coach
      description: Get a coach record by id.
      operationId: fetchCoach
      x-api-path-slug: coachid-get
      parameters:
      - in: path
        name: id
        description: Coach identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Coach
  /email_history:
    get:
      summary: List email histories
      description: Get a list of email histories
      operationId: fetchEmailHistories
      x-api-path-slug: email-history-get
      parameters:
      - in: query
        name: filter[emailType]
        description: Type of email
      - in: query
        name: filter[receiver]
        description: Twine user id of email recipient
      - in: query
        name: filter[sender]
        description: Twine user id of email sender
      - in: query
        name: sort
        description: 'valid sorts:  * send_time - ascending by send_time  * -send_time
          - descending by send_time'
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Email
      - Histories
  /email_history/{id}:
    get:
      summary: Get an email history
      description: Get an email history by id
      operationId: fetchEmailHistory
      x-api-path-slug: email-historyid-get
      parameters:
      - in: path
        name: id
        description: Email history identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Email
      - History
  /group:
    get:
      summary: List groups
      description: Get a list of groups matching the specified filters.
      operationId: fetchGroups
      x-api-path-slug: group-get
      parameters:
      - in: query
        name: filter[name]
        description: Group name
      - in: query
        name: filter[organization]
        description: Organization identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Groups
    post:
      summary: Create a group
      description: Create a group record.
      operationId: createGroup
      x-api-path-slug: group-post
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
      - Group
  /group/{id}:
    get:
      summary: Get a group
      description: Get a group record by id.
      operationId: fetchGroup
      x-api-path-slug: groupid-get
      parameters:
      - in: path
        name: id
        description: Group identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Group
  /health_profile:
    get:
      summary: List health profiles
      description: Get a list of health profiles
      operationId: fetchHealthProfiles
      x-api-path-slug: health-profile-get
      parameters:
      - in: query
        name: filter[groups]
        description: Comma-separated list of group ids
      - in: query
        name: filter[organization]
        description: Twine organization id
      - in: query
        name: filter[patient]
        description: Patient id to fetch health profile
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
      - Health
      - Profiles
  /health_profile/{id}:
    get:
      summary: Get a health profile
      description: Get a health profile by id
      operationId: fetchHealthProfile
      x-api-path-slug: health-profileid-get
      parameters:
      - in: path
        name: id
        description: Health profile identifier
      - in: query
        name: include
        description: List of related resources to include in the response
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Health
      - Profile
  /health_profile_answer:
    get:
      summary: List health profile answers
      description: Get a list of health profile answers
      operationId: fetchHealthProfileAnswers
      x-api-path-slug: health-profile-answer-get
      parameters:
      - in: query
        name: filter[groups]
        description: Comma-separated list of group ids
      - in: query
        name: filter[organization]
        description: Twine organization id
      - in: query
        name: filter[patient]
        description: Patient id to fetch healt profile answers
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
      - Health
      - Profile
      - Answers
  /health_profile_answer/{id}:
    get:
      summary: Get a health profile answer
      description: Get a health profile answer by id
      operationId: fetchHealthProfileAnswer
      x-api-path-slug: health-profile-answerid-get
      parameters:
      - in: path
        name: id
        description: Health profile answer identifier
      - in: query
        name: include
        description: List of related resources to include in the response
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Health
      - Profile
      - Answer
  /health_profile_question/{id}:
    get:
      summary: Get a health profile question
      description: Get a health profile by id
      operationId: fetchHealthProfileQuestion
      x-api-path-slug: health-profile-questionid-get
      parameters:
      - in: path
        name: id
        description: Health profile question identifier
      - in: query
        name: include
        description: List of related resources to include in the response
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Health
      - Profile
      - Question
  /health_question_definition:
    get:
      summary: List health question definitions
      description: Get a list of all health question definitions
      operationId: fetchHealthQuestionDefinitions
      x-api-path-slug: health-question-definition-get
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Health
      - Question
      - Definitions
  /health_question_definition/{id}:
    get:
      summary: Get a health question definition
      description: Get a health question definition by id
      operationId: fetchHealthQuestionDefinition
      x-api-path-slug: health-question-definitionid-get
      parameters:
      - in: path
        name: id
        description: Health question definition identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Health
      - Question
      - Definition
  /oauth/token:
    post:
      summary: Create an oauth token
      description: |-
        Create an OAuth 2.0 Bearer token. A valid bearer token is required for all other API requests.

        Be sure to set the header `Content-Type: "application/vnd.api+json"`. Otherwise, you will get an error
        403 Forbidden. Using `Content-Type: "application/json"` is permitted (to support older oauth clients) but when
        using `application/json` the body should have a body in the following format instead of nesting under
        `data.attributes`:
        ```
        {
          "grant_type": "client_credentials",
          "client_id": "95c78ab2-167f-40b8-8bec-8398d4b87454",
          "client_secret": "35d18dc9-a3dd-4948-b787-063a490b9354"
        }
        ```
      operationId: createToken
      x-api-path-slug: oauthtoken-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: include
        description: List of related resources to include in the response
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Oauth
      - Token
  /oauth/token/{id}/groups:
    get:
      summary: Get the groups for a token
      description: Get the list of groups a token can be used to access.
      operationId: fetchTokenGroups
      x-api-path-slug: oauthtokenidgroups-get
      parameters:
      - in: path
        name: id
        description: Token identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Groupsa
      - Token
  /oauth/token/{id}/organization:
    get:
      summary: Get the organization for a token
      description: Get the organization a token can be used to access.
      operationId: fetchTokenOrganization
      x-api-path-slug: oauthtokenidorganization-get
      parameters:
      - in: path
        name: id
        description: Token identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Organizationa
      - Token
  /organization/{id}:
    get:
      summary: Get an organization
      description: Get an organization record by id.
      operationId: fetchOrganization
      x-api-path-slug: organizationid-get
      parameters:
      - in: path
        name: id
        description: Organization identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Organization
  /patient:
    get:
      summary: List patients
      description: Get a list of patients.
      operationId: fetchPatients
      x-api-path-slug: patient-get
      parameters:
      - in: query
        name: filter[archived]
        description: If not specified, return all patients
      - in: query
        name: filter[created_at]
        description: The start (inclusive) and end (exclusive) dates are ISO date
          and time strings separated by `
      - in: query
        name: filter[groups]
        description: Comma-separated list of group ids
      - in: query
        name: filter[identifier][system]
        description: 'Identifier system (example: MyEHR) - requires a filter[identifier][value]
          parameter'
      - in: query
        name: filter[identifier][value]
        description: 'Identifier value (example: 12345) - requires a filter[identifier][system]
          parameter'
      - in: query
        name: filter[organization]
        description: Twine organization id
      - in: query
        name: filter[updated_at]
        description: The start (inclusive) and end (exclusive) dates are ISO date
          and time strings separated by `
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
      - Patients
    post:
      summary: Create a patient
      description: |-
        Create a patient record.

        Example for creating a patient with a group specified using `meta.query` instead of `id`:

        ```JSON
        {
          "data": {
            "type": "patient",
            "attributes": {
              "first_name": "Andrew",
              "last_name": "Smith"
            },
            "relationships": {
              "groups": {
                "data": [
                  {
                    "type": "group",
                    "meta": {
                      "query": {
                        "organization": "58c88de7c93eb96357a87033",
                        "name": "Patients Lead"
                      }
                    }
                  }
                ]
              }
            }
          }
        }
        ```
      operationId: createPatient
      x-api-path-slug: patient-post
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
      - Patient
  /patient/{id}:
    get:
      summary: Get a patient
      description: Gets a patient record by id.
      operationId: fetchPatient
      x-api-path-slug: patientid-get
      parameters:
      - in: path
        name: id
        description: Patient identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Patient
    patch:
      summary: Update a patient
      description: Update a patient record.
      operationId: updatePatient
      x-api-path-slug: patientid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Patient identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Patient
  /patient/{id}/coaches:
    get:
      summary: List coaches for a patient
      description: Get the list of coaches for a patient.
      operationId: fetchPatientCoaches
      x-api-path-slug: patientidcoaches-get
      parameters:
      - in: path
        name: id
        description: Patient identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Coachesa
      - Patient
  /patient/{id}/groups:
    get:
      summary: List groups for a patient
      description: Get the list of groups for a patient.
      operationId: fetchPatientGroups
      x-api-path-slug: patientidgroups-get
      parameters:
      - in: path
        name: id
        description: Patient identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Groupsa
      - Patient
  /patient_health_metric:
    get:
      summary: List patient health metrics
      description: Get a list of patient health metrics.
      operationId: fetchPatientHealthMetrics
      x-api-path-slug: patient-health-metric-get
      parameters:
      - in: query
        name: filter[patient]
        description: Filter the patient health metrics for a specified patient
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
      - Patient
      - Health
      - Metrics
    post:
      summary: Create patient health metrics
      description: |-
        Create one or more patient health metrics.

        Example for creating a patient health result with a patient specified using `meta.query` instead of `id`:

        ```JSON
          {
            "data": {
              "type": "patient_health_metric",
               "attributes": {
                 "code": {
                   "system": "LOINC",
                   "value": "13457-7"
                 },
                 "type": "ldl_cholesterol",
                 "occurred_at": "2017-03-14T11:00:57.000Z",
                 "value": "121",
                 "unit": "mg/dl"
              },
              "relationships": {
                "patient": {
                  "data": {
                    "type": "patient",
                    "meta": {
                      "query": {
                        "identifier": {
                          "system": "medical-record-number",
                          "value": "121212"
                        },
                        "organization": "58c4554710123c5c40dbab81"
                      }
                    }
                  }
                }
              }
            }
          }
        ```
      operationId: createPatientHealthMetric
      x-api-path-slug: patient-health-metric-post
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
      - Patient
      - Health
      - Metrics
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