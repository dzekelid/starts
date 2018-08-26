---
swagger: "2.0"
x-collection-name: Fitbit
x-complete: 0
info:
  title: Fitbit Get User User Activities Calories Date Start Date Or End Date End
    Date Or Period .json
  description: Get time series in the specified range for a given resource in the
    format requested using units in the unit system which corresponds to the Accept-Language
    header provided.
  version: 1.0.0
host: api.fitbit.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/{user-id}/sleep/minutesAsleep/date/{start-date-or-end-date}/{end-date-or-period}.json:
    get:
      summary: Get User User Sleep Minutesasleep Date Start Date Or End Date End Date
        Or Period .json
      description: Get time series in the specified range for a given resource in
        the format requested using units in the unit system which corresponds to the
        Accept-Language header provided.
      operationId: getUserUserSleepMinutesasleepDateStartDateOrEndDateEndDateOrPeriod.json
      x-api-path-slug: useruseridsleepminutesasleepdatestartdateorenddateenddateorperiod-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Sleep
      - MinutesAsleep
      - Date
      - Start-date-or-end-date
      - End-date-or-period.json
  /user/{user-id}/foods/log/caloriesIn/date/{start-date-or-end-date}/{end-date-or-period}.json:
    get:
      summary: Get User User Foods Log Caloriesin Date Start Date Or End Date End
        Date Or Period .json
      description: Get time series in the specified range for a given resource in
        the format requested using units in the unit system which corresponds to the
        Accept-Language header provided.
      operationId: getUserUserFoodsLogCaloriesinDateStartDateOrEndDateEndDateOrPeriod.json
      x-api-path-slug: useruseridfoodslogcaloriesindatestartdateorenddateenddateorperiod-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Foods
      - Log
      - CaloriesIn
      - Date
      - Start-date-or-end-date
      - End-date-or-period.json
  /user/{user-id}/body/weight/date/{start-date-or-end-date}/{end-date-or-period}.json:
    get:
      summary: Get User User Body Weight Date Start Date Or End Date End Date Or Period
        .json
      description: Get time series in the specified range for a given resource in
        the format requested using units in the unit system which corresponds to the
        Accept-Language header provided.
      operationId: getUserUserBodyWeightDateStartDateOrEndDateEndDateOrPeriod.json
      x-api-path-slug: useruseridbodyweightdatestartdateorenddateenddateorperiod-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Body
      - Weight
      - Date
      - Start-date-or-end-date
      - End-date-or-period.json
  /user/{user-id}/activities/calories/date/{start-date-or-end-date}/{end-date-or-period}.json:
    get:
      summary: Get User User Activities Calories Date Start Date Or End Date End Date
        Or Period .json
      description: Get time series in the specified range for a given resource in
        the format requested using units in the unit system which corresponds to the
        Accept-Language header provided.
      operationId: getUserUserActivitiesCaloriesDateStartDateOrEndDateEndDateOrPeriod.json
      x-api-path-slug: useruseridactivitiescaloriesdatestartdateorenddateenddateorperiod-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Activities
      - Calories
      - Date
      - Start-date-or-end-date
      - End-date-or-period.json
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