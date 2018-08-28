swagger: "2.0"
x-collection-name: GoToMeeting
x-complete: 1
info:
  title: SCIM
  description: the-scim-api-lets-you-manage-users-in-your-organization--you-can-then-automate-the-provisioning-of-product-licenses-for-these-users-and-they-can-use-your-companys-single-signon-solution-through-an-identity-provider-
  termsOfService: https://developer.citrixonline.com/terms-use
  contact:
    name: Developer Support
    url: https://developer.citrixonline.com
    email: developer-support@citrixonline.com
  version: N/A
host: api.citrixonline.com
basePath: /identity/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /meetings/{meetingId}/start:
    get:
      summary: Start meeting
      description: Returns a host URL that can be used to start a meeting. When this
        URL is opened in a web browser, the GoToMeeting client will be downloaded
        and launched and the meeting will start. The end user is not required to login
        to a client.
      operationId: returns-a-host-url-that-can-be-used-to-start-a-meeting--when-this-url-is-opened-in-a-web-browser-the
      x-api-path-slug: meetingsmeetingidstart-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Meetings
      - MeetingId
      - Start
  /trainings/{trainingKey}/start:
    get:
      summary: Start Training
      description: Returns a URL that can be used to start a training. When this URL
        is opened in a web browser, the GoToTraining client will be downloaded and
        launched and the training will start. A login of the organizer is not required.
      operationId: startTraining
      x-api-path-slug: trainingstrainingkeystart-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Trainings
      - TrainingKey
      - Start