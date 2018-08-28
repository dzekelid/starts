swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 1
info:
  title: GoToWebinar API
  description: todo-add-description
  version: 1.0.0
host: api.getgo.com
basePath: /G2W/rest/organizers
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /sessions:
    post:
      summary: Start Screen Sharing Session
      description: "This method creates a new screen sharing support session (either
        attended or unattended) by generating a URL that automatically launches technicians
        into a new session when clicked. If a machineUuid request parameter is specified,
        an unattended support session will be created; if it is not specified, then
        an attended session will be created. See \"Request Parameters\" for more information.
        Note: The locale of the session start dialog will be based upon the technician\u2019s
        locale setting within GoToAssist.\n\nNote: This method was formerly named
        \"Create Attended Session,\" but has been renamed to address the fact that
        it now includes unattended support sessions as well.\n\n  Request Parameters
        \                   \n                      \n    field        data type      description
        \   \n    sessionStatusCallbackUrl*        string      The URL that will receive
        a POST when the session status changes. A POST will also be made to the sessionStatusCallbackUrl
        when a customer joins the session and when the session ends (whether or not
        a customer joined). The contents of the POST will be similar as the GET /v1/sessions/
        API. Note: The ID of the session is not known until the session is actually
        started on the endpoint. If the URL is not specified or the session is never
        started (e.g., if the customer cancels the installation of the GoToAssist
        Customer desktop application), then the callback will not be made.    \n    sessionType
        \       string      The type of session to create (only \"SCREEN_SHARING\"
        can be used at this time).    \n    partnerObject*        string      The
        ID of object in the partner system that this session will be associated with.
        \   \n    partnerObjectUrl*        string      The URL that may be used in
        the GoToAssist Expert desktop application if the technician wants to view
        the partner object. Note: The URL can be used in a popup window or iframe
        that is 600 pixels wide and 500 pixels wide. For example, a popup window could
        be created with HTML code as follows: \"Start Remote Support \"    \n    customerName*
        \       string      The name of the customer that the session is being started
        for.    \n    customerEmail*        string      The email address of the customer
        that the session is being started for (if available)    \n    machineUuid*
        \       string      The machineUuid is only necessary for unattended support
        sessions. If the machineUuid is present when a screen sharing session is started,
        then the endpoint will connect to the specified unattended machine and an
        unattended support session will be started. If no machineUuid is specified,
        then an attended support session will be created. A list of machineUuid parameters
        associated with the user and company will be available through a /machines
        API in future.    \n                      \n* Optional parameters\n\nStatus
        Codes              \n              \n    Staus Code      description    \n
        \   200 OK      The response contains the URL to start the session    \n    400
        Bad Request      An error occurred due to missing required parameters or portal
        not being created    \n    401 Unauthorized      An authentication parameter
        was passed, but either it was invalid or the technician is not entitled with
        a Remote Support seat    \n    403 Forbidden      Access denied. User doesn\u2019t
        have required roles    \n    404 Not Found      A machineUuid was specified,
        but the specified machine was not found in an account the user has access
        to    \n    405 Method Not Allowed      The method was entered incorrectly
        (i.e., the technician tried to use POST, PUT etc. instead of GET)    \n    500
        Internal Server Error      An unhandled error occurred"
      operationId: SessionsPost2
      x-api-path-slug: sessions-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Start
      - Screen
      - Sharing
      - Session
  /session:
    get:
      summary: Start Attended Session in Browser
      description: "This method allows a partner system to launch an attended support
        session within a browser window. This API does not require authentication,
        so the technician will be prompted to enter their credentials when they run
        the GoToAssist Expert desktop application for the first time. Since the technician
        is not required to navigate to a URL, no API is implemented to create the
        session. Note: This method was formerly named \"Create Attended Session in
        browser,\" but has been renamed.\n\n  Request Parameters                    \n
        \                     \n    field        data type      description    \n
        \   sessionType        string      The type of session to create (only \"SCREEN_SHARING\"
        can be used at this time).    \n    layout*        string      The style of
        HTML that will be displayed when starting the session (e.g., \"iFrame\").
        If this parameter is not present, then the HTML will fill the entire browser
        window.    \n    partnerObject*        string      The ID of object in the
        partner system that this session will be associated with.    \n    partnerObjectUrl*
        \       string      The URL that may be used in the GoToAssist Expert desktop
        application if the technician wants to view the partner object. Note: The
        URL can be used in a popup window or iframe that is 600 pixels wide and 500
        pixels wide. For example, a popup window could be created with HTML code as
        follows: Start Remote Support     \n    sessionStatusCallbackUrl*        string
        \     The URL that will receive a POST when the session status changes. A
        POST will also be made to the sessionStatusCallbackUrl when a customer joins
        the session and when the session ends (whether or not a customer joined).
        The contents of the POST will be similar as the GET /v1/sessions/ API. Note:
        The ID of the session is not known until the session is actually started on
        the endpoint. If the URL is not specified or the session is never started
        (e.g., if the customer cancels the installation of the GoToAssist Customer
        desktop application), then the callback will not be made.    \n                      \n*
        Optional parameters"
      operationId: SessionGet
      x-api-path-slug: session-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: sessionType
      responses:
        200:
          description: OK
      tags:
      - Start
      - Attended
      - Session
      - In
      - Browser
  /archive/recordings/urls[&{attribute}={readyForDownloadRecordingId}]:
    get:
      summary: Download Recordings
      description: "This method retrieves download links for a list of recordings.
        Each recording returns a link to the MP4 file, the .events file and the thumbnail.
        If a recording is not available for download then it will be omitted from
        the returned list. The archiving script may use the returned URLs to download
        each resource for the recording. The URLs will be valid for at least 48 hours.
        The URL contains a large random number so that the URL for recordings cannot
        be guessed. The response includes the recording start time to make it easier
        for the archiving script to place recordings in directories based on date.
        No more than 500 recordings can be requested at once.\n\nNote: Session recording
        must be enabled on the account in order to use this API method. To enable
        session recording, log in at https://app.gotoassist.com (link is external)
        and go to Configure > GoToAssist Settings > Enable Session Recording check
        box.\n\n  Response Parameters                  \n                    \n    field
        \     data type      description    \n    recordingId      number      The
        recordingId of the session recording to be downloaded    \n    recordingUrl
        \     string      The URL of MP4 recording file    \n    recordingStartTime
        \     ISO 8601 format*      The start time of recording    \n    eventsUrl
        \     string      The URL of the events recording file    \n    thumbnailUrl
        \     string      The URL of the thumbnail of recording file    \n    recordingSize
        \     string      The size of the .mp4 file in bytes    \n\n* ISO 8601 format
        reference\n                    \nStatus Codes                    \n                    \n
        \   Staus Code      description          \n    200 OK      A list of URLs
        has been returned          \n    400 Bad Request      Request may be malformed
        or property may be missing or invalid          \n    403 Forbidden      Invalid
        authorization header or invalid recording Ids          \n    500 Internal
        Server Error      Unexpected server error"
      operationId: ArchiveRecordingsUrlsAPIGet
      x-api-path-slug: archiverecordingsurlsattributereadyfordownloadrecordingid-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: attribute
      - in: header
        name: Content-Type
      - in: path
        name: readyForDownloadRecordingId
      responses:
        200:
          description: OK
      tags:
      - Download
      - Recordings
  /trainings/{trainingKey}/start:
    get:
      summary: Start Training
      description: Start training.
      operationId: TrainingsStartByTrainingKeyGet
      x-api-path-slug: trainingstrainingkeystart-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: trainingKey
      responses:
        200:
          description: OK
      tags:
      - Start
      - Training
  /organizers/{organizerKey}/trainings/{trainingKey}/startUrl:
    get:
      summary: Get Start Url
      description: Get start url.
      operationId: OrganizersTrainingsStartUrlByOrganizerKeyAndTrainingKeyGet
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeystarturl-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: trainingKey
      responses:
        200:
          description: OK
      tags:
      - Start
      - Url