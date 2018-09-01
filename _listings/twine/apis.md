---
name: Twine
x-slug: twine
description: 'Twine Health is a cloud-based collaborative care platform for chronic
  disease management. It consists of a patient engagement portal, a peer support network,
  a care management solution, and an outcome analytics tool. The platform enables
  users to co-create personalized care plans that serve as common ground for collaboration
  with their care team: their own providers such as physicians and nurse practitioners;
  their family and friends; and coaches such as nurses, pharmacists, health coaches,
  and more.'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Twine
created: "2018-08-31"
modified: "2018-08-31"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/apis.md
specificationVersion: "0.14"
apis:
- name: Twine - Create action
  x-api-slug: action-post
  description: Create a plan action
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/action-post-openapi.md
- name: Twine - Get an action
  x-api-slug: actionid-get
  description: Get a health action from a patient's plan.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/actionid-get-openapi.md
- name: Twine - Update an action
  x-api-slug: actionid-patch
  description: Update a health action from a patient's plan.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/actionid-patch-openapi.md
- name: Twine - Create bundle
  x-api-slug: bundle-post
  description: Create a bundle in a patient's plan
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/bundle-post-openapi.md
- name: Twine - Get a bundle
  x-api-slug: bundleid-get
  description: Get a bundle from a patient's plan.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/bundleid-get-openapi.md
- name: Twine - Update a bundle
  x-api-slug: bundleid-patch
  description: Updte a bundle from a patient's plan.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/bundleid-patch-openapi.md
- name: Twine - List calendar events
  x-api-slug: calendar-event-get
  description: Get a list of calendar events
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/calendar-event-get-openapi.md
- name: Twine - Create calendar event
  x-api-slug: calendar-event-post
  description: Create a calendar event for a patient. Attribute `all_day` must be
    set to `true` and `end_at` cannot be set for `plan-check-in` event type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/calendar-event-post-openapi.md
- name: Twine - Delete a calendar event
  x-api-slug: calendar-eventid-delete
  description: Delete a calendar event by id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/calendar-eventid-delete-openapi.md
- name: Twine - Get a calendar event
  x-api-slug: calendar-eventid-get
  description: Get a calendar event by id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/calendar-eventid-get-openapi.md
- name: Twine - Update a calendar event
  x-api-slug: calendar-eventid-patch
  description: Update a calendar event for a patient. Attribute `all_day` must be
    true and `end_at` cannot be specified for `plan-check-in` event type. To mark
    a calendar event as 'completed', set `completed_at` and `completed_by` to desired
    values.  To mark a completed calendar event as 'not completed', set `completed_at`
    and `completed_by` to `null`.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/calendar-eventid-patch-openapi.md
- name: Twine - Get a coach
  x-api-slug: coachid-get
  description: Get a coach record by id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/coachid-get-openapi.md
- name: Twine - List email histories
  x-api-slug: email-history-get
  description: Get a list of email histories
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/email-history-get-openapi.md
- name: Twine - Get an email history
  x-api-slug: email-historyid-get
  description: Get an email history by id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/email-historyid-get-openapi.md
- name: Twine - List groups
  x-api-slug: group-get
  description: Get a list of groups matching the specified filters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/group-get-openapi.md
- name: Twine - Create a group
  x-api-slug: group-post
  description: Create a group record.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/group-post-openapi.md
- name: Twine - Get a group
  x-api-slug: groupid-get
  description: Get a group record by id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/groupid-get-openapi.md
- name: Twine - List health profiles
  x-api-slug: health-profile-get
  description: Get a list of health profiles
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/health-profile-get-openapi.md
- name: Twine - Get a health profile
  x-api-slug: health-profileid-get
  description: Get a health profile by id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/health-profileid-get-openapi.md
- name: Twine - List health profile answers
  x-api-slug: health-profile-answer-get
  description: Get a list of health profile answers
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/health-profile-answer-get-openapi.md
- name: Twine - Get a health profile answer
  x-api-slug: health-profile-answerid-get
  description: Get a health profile answer by id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/health-profile-answerid-get-openapi.md
- name: Twine - Get a health profile question
  x-api-slug: health-profile-questionid-get
  description: Get a health profile by id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/health-profile-questionid-get-openapi.md
- name: Twine - List health question definitions
  x-api-slug: health-question-definition-get
  description: Get a list of all health question definitions
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/health-question-definition-get-openapi.md
- name: Twine - Get a health question definition
  x-api-slug: health-question-definitionid-get
  description: Get a health question definition by id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/health-question-definitionid-get-openapi.md
- name: Twine - Create an oauth token
  x-api-slug: oauthtoken-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/oauthtoken-post-openapi.md
- name: Twine - Get the groups for a token
  x-api-slug: oauthtokenidgroups-get
  description: Get the list of groups a token can be used to access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/oauthtokenidgroups-get-openapi.md
- name: Twine - Get the organization for a token
  x-api-slug: oauthtokenidorganization-get
  description: Get the organization a token can be used to access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/oauthtokenidorganization-get-openapi.md
- name: Twine - Get an organization
  x-api-slug: organizationid-get
  description: Get an organization record by id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/organizationid-get-openapi.md
- name: Twine - List patients
  x-api-slug: patient-get
  description: Get a list of patients.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/patient-get-openapi.md
- name: Twine - Create a patient
  x-api-slug: patient-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/patient-post-openapi.md
- name: Twine - Get a patient
  x-api-slug: patientid-get
  description: Gets a patient record by id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/patientid-get-openapi.md
- name: Twine - Update a patient
  x-api-slug: patientid-patch
  description: Update a patient record.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/patientid-patch-openapi.md
- name: Twine - List coaches for a patient
  x-api-slug: patientidcoaches-get
  description: Get the list of coaches for a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/patientidcoaches-get-openapi.md
- name: Twine - List groups for a patient
  x-api-slug: patientidgroups-get
  description: Get the list of groups for a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/patientidgroups-get-openapi.md
- name: Twine - List patient health metrics
  x-api-slug: patient-health-metric-get
  description: Get a list of patient health metrics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/patient-health-metric-get-openapi.md
- name: Twine - Create patient health metrics
  x-api-slug: patient-health-metric-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/patient-health-metric-post-openapi.md
- name: Twine - Get a patient health metric
  x-api-slug: patient-health-metricid-get
  description: Get the plan summary for a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/patient-health-metricid-get-openapi.md
- name: Twine - List patient plan summaries
  x-api-slug: patient-plan-summary-get
  description: Get a list of patient plan summaries
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/patient-plan-summary-get-openapi.md
- name: Twine - Get the plan summary for a patient
  x-api-slug: patient-plan-summaryid-get
  description: Get the plan summary for a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/patient-plan-summaryid-get-openapi.md
- name: Twine - Update a plan summary
  x-api-slug: patient-plan-summaryid-patch
  description: Update a plan summary record for a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/patient-plan-summaryid-patch-openapi.md
- name: Twine - List rewards
  x-api-slug: reward-get
  description: Get a list of rewards matching the specified filters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/reward-get-openapi.md
- name: Twine - Create a reward
  x-api-slug: reward-post
  description: Create a reward for a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/reward-post-openapi.md
- name: Twine - Get a reward
  x-api-slug: rewardid-get
  description: Get a reward record by id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/rewardid-get-openapi.md
- name: Twine - List reward earnings
  x-api-slug: reward-earning-get
  description: Get a list of reward earnings matching the specified filters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/reward-earning-get-openapi.md
- name: Twine - Create a reward earning
  x-api-slug: reward-earning-post
  description: Create a reward earning for a reward. There can only be one earning
    for a reward. It is possilble to create multiple reward earnings simultaneously
    by providing and array of reward earnings in the data property.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/reward-earning-post-openapi.md
- name: Twine - Get a reward earning
  x-api-slug: reward-earningid-get
  description: Get a reward earning record by id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/reward-earningid-get-openapi.md
- name: Twine - List reward earning fulfillments
  x-api-slug: reward-earning-fulfillment-get
  description: Get a list of reward earning fulfillments matching the specified filters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/reward-earning-fulfillment-get-openapi.md
- name: Twine - Create a reward earning fulfillment
  x-api-slug: reward-earning-fulfillment-post
  description: Create a reward earning fulfillment for a reward earning. There can
    only be one fulfillment for each earning.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/reward-earning-fulfillment-post-openapi.md
- name: Twine - Get a reward earning fulfillment
  x-api-slug: reward-earning-fulfillmentid-get
  description: Get a reward earning fulfillment record by id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/reward-earning-fulfillmentid-get-openapi.md
- name: Twine - List reward programs
  x-api-slug: reward-program-get
  description: Get a list of reward programs matching the specified filters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/reward-program-get-openapi.md
- name: Twine - Create a reward program
  x-api-slug: reward-program-post
  description: Create a reward program for a group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/reward-program-post-openapi.md
- name: Twine - Get a reward program
  x-api-slug: reward-programid-get
  description: Get a reward program record by id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/reward-programid-get-openapi.md
- name: Twine - Get group for a reward program
  x-api-slug: reward-programidgroup-get
  description: Get the group related to a reward program.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/reward-programidgroup-get-openapi.md
- name: Twine - List reward program activations
  x-api-slug: reward-program-activation-get
  description: Get a list of reward program activations matching the specified filters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/reward-program-activation-get-openapi.md
- name: Twine - Create a reward program activation
  x-api-slug: reward-program-activation-post
  description: Create a reward program activation for a patient. There can only be
    one activation for a patient for a given reward program.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/reward-program-activation-post-openapi.md
- name: Twine - Get a reward program activation
  x-api-slug: reward-program-activationid-get
  description: Get a reward program activationrecord by id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twine/master/_listings/twine/reward-program-activationid-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://twilio.api.gallery.streamdata.io
- type: x-api-stack
  url: http://twine.stack.network
- type: x-authentication
  url: http://developer.twinehealth.com/#section/Authentication
- type: x-developer
  url: http://developer.twinehealth.com/
- type: x-website
  url: http://twinehealth.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---