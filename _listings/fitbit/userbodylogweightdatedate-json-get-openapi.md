---
swagger: "2.0"
x-collection-name: Fitbit
x-complete: 0
info:
  title: Fitbit Get User Body Log Weight Date Date .json
  description: Get a list of all user's body weight log entries for a given day in
    the format requested using units in the unit system which corresponds to the Accept-Language
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
  /user/-/body/log/weight/goal.json:
    post:
      summary: Post User Body Log Weight Goal.json
      description: Create or update user's weight goal using units in the unit system
        that corresponds to the Accept-Language header provided and get a response
        in the format requested.
      operationId: postUserBodyLogWeightGoal.json
      x-api-path-slug: userbodylogweightgoal-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Body
      - Log
      - Weight
      - Goal.json
    get:
      summary: Get User Body Log Weight Goal.json
      description: Get a user's current weight goal using units in the unit system
        that corresponds to the Accept-Language header provided in the format requested.
      operationId: getUserBodyLogWeightGoal.json
      x-api-path-slug: userbodylogweightgoal-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Body
      - Log
      - Weight
      - Goal.json
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
  /user/-/body/log/weight/date/{date}.json:
    get:
      summary: Get User Body Log Weight Date Date .json
      description: Get a list of all user's body weight log entries for a given day
        in the format requested using units in the unit system which corresponds to
        the Accept-Language header provided.
      operationId: getUserBodyLogWeightDateDate.json
      x-api-path-slug: userbodylogweightdatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Body
      - Log
      - Weight
      - Date
      - Date.json
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