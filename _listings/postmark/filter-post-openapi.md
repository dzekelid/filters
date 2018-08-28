---
swagger: "2.0"
x-collection-name: Postmark
x-complete: 0
info:
  title: Postmark Post Filter
  description: 'Postmark???s spam API is a RESTfull interface to the Spam filter tool
    SpamAssassin (http://spamassassin.apache.org/). This can be used to pre or post
    process email content when it is used in your application. For instance, if you
    process incoming emails from your users you can first run it through the API to
    filter out junk and avoid clutter in your database and application. Keep in mind:
    This is free to use and may be updated, removed or changed at any time. For a
    detailed explanation of the report generated, as well as the test definitions,
    please visit the SpamAssassin test repository (http://spamassassin.apache.org/tests_3_3_x.html).
    The POST body must have an element "email" which is the raw dump of the email
    to be filtered, including all headers. And an element "options" which must either
    be "long" for a full report of processing rules, or "short" for a score request.'
  version: 1.0.0
host: spamcheck.postmarkapp.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /filter:
    post:
      summary: Post Filter
      description: 'Postmark???s spam API is a RESTfull interface to the Spam filter
        tool SpamAssassin (http://spamassassin.apache.org/). This can be used to pre
        or post process email content when it is used in your application. For instance,
        if you process incoming emails from your users you can first run it through
        the API to filter out junk and avoid clutter in your database and application.
        Keep in mind: This is free to use and may be updated, removed or changed at
        any time. For a detailed explanation of the report generated, as well as the
        test definitions, please visit the SpamAssassin test repository (http://spamassassin.apache.org/tests_3_3_x.html).
        The POST body must have an element "email" which is the raw dump of the email
        to be filtered, including all headers. And an element "options" which must
        either be "long" for a full report of processing rules, or "short" for a score
        request.'
      operationId: postFilter
      x-api-path-slug: filter-post
      parameters:
      - in: query
        name: Accept
        description: The accepted type for the response
      - in: query
        name: Content-Type
        description: The content type of the request
      responses:
        200:
          description: OK
      tags:
      - Filter
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