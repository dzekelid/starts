---
name: LogMeIn
x-slug: logmein
description: LogMeIn, Inc. is a provider of software as a service and cloud-based
  remote connectivity services for collaboration, IT management and customer engagement,
  founded in 2003 and based in Boston, Massachusetts.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
x-kinRank: "7"
x-alexaRank: "7271"
tags: Starts
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/starts/master/_listings/logmein/apis.md
specificationVersion: "0.14"
apis:
- name: GoToAssist Remote Support - Start Attended Session in Browser
  x-api-slug: session-get
  description: "This method allows a partner system to launch an attended support
    session within a browser window. This API does not require authentication, so
    the technician will be prompted to enter their credentials when they run the GoToAssist
    Expert desktop application for the first time. Since the technician is not required
    to navigate to a URL, no API is implemented to create the session. Note: This
    method was formerly named \"Create Attended Session in browser,\" but has been
    renamed.\n\n  Request Parameters                    \n                      \n
    \   field        data type      description    \n    sessionType        string
    \     The type of session to create (only \"SCREEN_SHARING\" can be used at this
    time).    \n    layout*        string      The style of HTML that will be displayed
    when starting the session (e.g., \"iFrame\"). If this parameter is not present,
    then the HTML will fill the entire browser window.    \n    partnerObject*        string
    \     The ID of object in the partner system that this session will be associated
    with.    \n    partnerObjectUrl*        string      The URL that may be used in
    the GoToAssist Expert desktop application if the technician wants to view the
    partner object. Note: The URL can be used in a popup window or iframe that is
    600 pixels wide and 500 pixels wide. For example, a popup window could be created
    with HTML code as follows: Start Remote Support     \n    sessionStatusCallbackUrl*
    \       string      The URL that will receive a POST when the session status changes.
    A POST will also be made to the sessionStatusCallbackUrl when a customer joins
    the session and when the session ends (whether or not a customer joined). The
    contents of the POST will be similar as the GET /v1/sessions/ API. Note: The ID
    of the session is not known until the session is actually started on the endpoint.
    If the URL is not specified or the session is never started (e.g., if the customer
    cancels the installation of the GoToAssist Customer desktop application), then
    the callback will not be made.    \n                      \n* Optional parameters"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2A/rest/v1
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/starts/master/_listings/logmein/session-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/starts/master/_listings/logmein/session-get-openapi.md
- name: GoToAssist Remote Support - Start Attended Session in Browser
  x-api-slug: session-get
  description: "This method allows a partner system to launch an attended support
    session within a browser window. This API does not require authentication, so
    the technician will be prompted to enter their credentials when they run the GoToAssist
    Expert desktop application for the first time. Since the technician is not required
    to navigate to a URL, no API is implemented to create the session. Note: This
    method was formerly named \"Create Attended Session in browser,\" but has been
    renamed.\n\n  Request Parameters                    \n                      \n
    \   field        data type      description    \n    sessionType        string
    \     The type of session to create (only \"SCREEN_SHARING\" can be used at this
    time).    \n    layout*        string      The style of HTML that will be displayed
    when starting the session (e.g., \"iFrame\"). If this parameter is not present,
    then the HTML will fill the entire browser window.    \n    partnerObject*        string
    \     The ID of object in the partner system that this session will be associated
    with.    \n    partnerObjectUrl*        string      The URL that may be used in
    the GoToAssist Expert desktop application if the technician wants to view the
    partner object. Note: The URL can be used in a popup window or iframe that is
    600 pixels wide and 500 pixels wide. For example, a popup window could be created
    with HTML code as follows: Start Remote Support     \n    sessionStatusCallbackUrl*
    \       string      The URL that will receive a POST when the session status changes.
    A POST will also be made to the sessionStatusCallbackUrl when a customer joins
    the session and when the session ends (whether or not a customer joined). The
    contents of the POST will be similar as the GET /v1/sessions/ API. Note: The ID
    of the session is not known until the session is actually started on the endpoint.
    If the URL is not specified or the session is never started (e.g., if the customer
    cancels the installation of the GoToAssist Customer desktop application), then
    the callback will not be made.    \n                      \n* Optional parameters"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2A/rest/v1
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/starts/master/_listings/logmein/session-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/starts/master/_listings/logmein/session-get-openapi.md
- name: GoToAssist Remote Support - Download Recordings
  x-api-slug: archiverecordingsurlsattributereadyfordownloadrecordingid-get
  description: "This method retrieves download links for a list of recordings. Each
    recording returns a link to the MP4 file, the .events file and the thumbnail.
    If a recording is not available for download then it will be omitted from the
    returned list. The archiving script may use the returned URLs to download each
    resource for the recording. The URLs will be valid for at least 48 hours. The
    URL contains a large random number so that the URL for recordings cannot be guessed.
    The response includes the recording start time to make it easier for the archiving
    script to place recordings in directories based on date. No more than 500 recordings
    can be requested at once.\n\nNote: Session recording must be enabled on the account
    in order to use this API method. To enable session recording, log in at https://app.gotoassist.com
    (link is external) and go to Configure > GoToAssist Settings > Enable Session
    Recording check box.\n\n  Response Parameters                  \n                    \n
    \   field      data type      description    \n    recordingId      number      The
    recordingId of the session recording to be downloaded    \n    recordingUrl      string
    \     The URL of MP4 recording file    \n    recordingStartTime      ISO 8601
    format*      The start time of recording    \n    eventsUrl      string      The
    URL of the events recording file    \n    thumbnailUrl      string      The URL
    of the thumbnail of recording file    \n    recordingSize      string      The
    size of the .mp4 file in bytes    \n\n* ISO 8601 format reference\n                    \nStatus
    Codes                    \n                    \n    Staus Code      description
    \         \n    200 OK      A list of URLs has been returned          \n    400
    Bad Request      Request may be malformed or property may be missing or invalid
    \         \n    403 Forbidden      Invalid authorization header or invalid recording
    Ids          \n    500 Internal Server Error      Unexpected server error"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2A/rest/v1
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/starts/master/_listings/logmein/archiverecordingsurlsattributereadyfordownloadrecordingid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/starts/master/_listings/logmein/archiverecordingsurlsattributereadyfordownloadrecordingid-get-openapi.md
- name: GoToTraining API - Start Training
  x-api-slug: trainingstrainingkeystart-get
  description: Start training.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2T/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/starts/master/_listings/logmein/trainingstrainingkeystart-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/starts/master/_listings/logmein/trainingstrainingkeystart-get-openapi.md
- name: GoToTraining API - Get Start Url
  x-api-slug: organizersorganizerkeytrainingstrainingkeystarturl-get
  description: Get start url.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2T/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/starts/master/_listings/logmein/organizersorganizerkeytrainingstrainingkeystarturl-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/starts/master/_listings/logmein/organizersorganizerkeytrainingstrainingkeystarturl-get-openapi.md
- name: GoToTraining API - Start Training
  x-api-slug: trainingstrainingkeystart-get
  description: Start training.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2T/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/starts/master/_listings/logmein/trainingstrainingkeystart-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/starts/master/_listings/logmein/trainingstrainingkeystart-get-openapi.md
- name: GoToTraining API - Get Start Url
  x-api-slug: organizersorganizerkeytrainingstrainingkeystarturl-get
  description: Get start url.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2T/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/starts/master/_listings/logmein/organizersorganizerkeytrainingstrainingkeystarturl-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/starts/master/_listings/logmein/organizersorganizerkeytrainingstrainingkeystarturl-get-openapi.md
x-common:
- type: x-github
  url: https://github.com/logmein
- type: x-openapi
  url: https://www.getpostman.com/collections/94ad52bdc3d954bad52a
- type: x-postman-collection
  url: https://www.getpostman.com/collections/00bf4391e993c3afa7b7
- type: x-postman-collection
  url: https://www.getpostman.com/collections/c35d614484f21e581775
- type: x-postman-collection
  url: https://www.getpostman.com/collections/9c6e067461f45f7faa6b
- type: x-postman-collection
  url: https://drive.google.com/open?id=16WZlBkS1i8cWSfZ3mMKOwlNP-qsE7AWy
- type: x-postman-collection
  url: https://drive.google.com/file/d/1vI11FNCKpv6WJ_70hoqPNMmPAkASiOU_/view?usp=sharing
- type: x-website
  url: http://www.LogMeInInc.com
- type: x-api-gallery
  url: http://loginradius.api.gallery.streamdata.io
- type: x-api-stack
  url: http://logmein.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/logmein
- type: x-developer
  url: https://goto-developer.logmeininc.com/
- type: x-documentation
  url: https://goto-developer.logmeininc.com/apis/apis-overview
- type: x-faq
  url: https://goto-developer.logmeininc.com/faq-page
- type: x-support
  url: https://goto-developer.logmeininc.com/api-support-request-template
- type: x-twitter
  url: https://twitter.com/LogMeIn
- type: x-website
  url: https://www.logmeininc.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---