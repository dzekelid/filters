swagger: "2.0"
x-collection-name: HERE
x-complete: 1
info:
  title: Weather API
  description: the-here-weather-api-provides-weather-forecasts-and-reports-on-current-weather-conditions-provides-information-on-severe-weather-alerts-provides-information-about-when-the-sun-and-moon-rise-and-set-and-the-phase-of-the-moonthis-example-set-works-with-version-1-2-4-or-higheradditional-information-can-be-found-on-developer-here-comhttpsdeveloper-here-comrestapisdocumentationweather
  version: 1.0.0
host: weather.cit.api.here.com
basePath: /weather/1.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /attribute:
    get:
      summary: Filtering by Custom Attributes
      description: |-
        *Request a list of user-defined locations based on their attribute values*

        An attribute-based search is requested using the `attribute` endpoint and by adding the `query` parameter to the request URL.



        * **layerId**  `text`
         \- Unique indicator used to retrieve a dataset

        * **query**  `text`
         \- The query to retrieve

        * **app_id**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

        * **app_code**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.
      operationId: AttributeGet
      x-api-path-slug: attribute-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: layerId
      - in: query
        name: query
      responses:
        200:
          description: OK
      tags:
      - Filtering
      - By
      - Custom
      - Attributes
  /maptile/newest/normal.day/16/18743/25072/256/png8:
    get:
      summary: Filtering Points of Interest
      description: "*Request a map tile including selected points of interest*\n\nPoints
        of interest are displayed by passing the `pois` parameter in the request URL.
        The type of points of interest to be displayed can be filtered by using a
        hexadecimal bitmask.\n  \n\n\n\n* **pois**  `text`\n \\- Displays points of
        interest if present  \n\n Valid values are : `default`, `alps`, `fleet`, `wings`,
        `dreamworks`, `flame`, `mini`\n\n* **app_id**  `text`\n \\- A 20 byte Base64
        URL-safe encoded string used for the authentication of the client application.
        \   You must include an `app_id` with every request.\n\n* **app_code**  `text`\n
        \\- A 20 byte Base64 URL-safe encoded string used for the authentication of
        the client application.    You must include an `app_code` with every request."
      operationId: MaptileNewestNormalDay161874325072256Png8Get3
      x-api-path-slug: maptilenewestnormal-day161874325072256png8-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: pois
      responses:
        200:
          description: OK
      tags:
      - Filtering
      - Points
      - Of
      - Interest
  /6.0/incidents.json:
    get:
      summary: Traffic Incidents via Proximity
      description: |-
        *Request traffic incident information within specified area*

        Traffic incidents can be retrieved through several different request types, based on the addressing schemes that they use to specify their geography. Traffic requests can be output to either XML or JSON format. API also supports filters to limit the amount of information provided in the response. Filters are based on on status, criticality, TMC table IDs, profiles, or start and end times, etc.



        * **prox**  `prox`
         \- A type of spatial filter. Proximity specifies a circle to search using a latitude, a longitude, and a radius in meters.    e.g. `52.515,13.377,100`

        * **criticality**  `multi-enum`
         \- A filter that selects incident reports according to criticality,  `0`=critical, `1`=major, `2`=minor,  `3`=lowImpact

         Valid values are : `0` - critical, `1` - major, `2` - minor, `3` - lowImpact

        * **app_id**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

        * **app_code**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.
      operationId: 60IncidentsJsonGet3
      x-api-path-slug: 6-0incidents-json-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: criticality
      - in: query
        name: prox
      responses:
        200:
          description: OK
      tags:
      - Traffic
      - Incidents
      - Via
      - Proximity