---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Save feedback follow up filter
  version: 1.0.0
  description: Save feedback follow up filter.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/list/followups/filters:
    get:
      summary: Get all saved follow up list filters
      description: Get all saved follow up list filters.
      operationId: List_GetFollowUpListFiltersByroleTypeBycontext
      x-api-path-slug: apilistfollowupsfilters-get
      parameters:
      - in: query
        name: context
        description: Filter context
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleType
        description: Filter roleType
      responses:
        200:
          description: OK
      tags:
      - Saved
      - Follow
      - Up
      - List
      - Filters
  /api/list/feedback/followups/filters:
    get:
      summary: Get all saved feedback follow up list filters
      description: Get all saved feedback follow up list filters.
      operationId: List_GetFeedbackFollowUpListFiltersByroleTypeBycontext
      x-api-path-slug: apilistfeedbackfollowupsfilters-get
      parameters:
      - in: query
        name: context
        description: Filter context
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleType
        description: Filter roleType
      responses:
        200:
          description: OK
      tags:
      - Saved
      - Feedback
      - Follow
      - Up
      - List
      - Filters
  /api/todo/getall:
    get:
      summary: "Get the list of all ToDo's if no parameter is sent;\r\n<param name=\"filterToDo\">if
        provided will filter by ToDo type</param><param name=\"pageSize\"></param><param
        name=\"pageNumber\"></param>"
      description: "Get the list of all todo's if no parameter is sent;\r\n<param
        name=\"filtertodo\">if provided will filter by todo type</param><param name=\"pagesize\"></param><param
        name=\"pagenumber\"></param>."
      operationId: DefaultToDo_GetAllBypageSizeBypageNumberByfilterToDo.filterCategoryByfilterToDo.toDoTypeByfilterToDo
      x-api-path-slug: apitodogetall-get
      parameters:
      - in: query
        name: filterToDo.branchId
      - in: query
        name: filterToDo.filterCategory
      - in: query
        name: filterToDo.negotiatorIds
      - in: query
        name: filterToDo.toDoType
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - ToDos
      - If
      - "No"
      - Parameter
      - Is
      - "Sent;\r\n<param"
      - Name=filterToDo>if
      - Provided
      - Will
      - Filter
      - By
      - ToDo
      - Type<
      - Param><param
      - Name=pageSize><
      - Param><param
      - Name=pageNumber><
      - Param>
  /api/list/events/filters/{id}:
    delete:
      summary: Marks Event List Filter as deleted
      description: Marks event list filter as deleted.
      operationId: List_DeleteEventFilterByid
      x-api-path-slug: apilisteventsfiltersid-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Event
      - List
      - Filter
      - As
      - Deleted
  /api/list/property/filters/{id}:
    delete:
      summary: Marks Property List Filter as deleted
      description: Marks property list filter as deleted.
      operationId: List_DeletePropertyFilterByid
      x-api-path-slug: apilistpropertyfiltersid-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Property
      - List
      - Filter
      - As
      - Deleted
  /api/list/groups/filters/{id}:
    delete:
      summary: Marks Groups List Filter as deleted
      description: Marks groups list filter as deleted.
      operationId: List_DeleteGroupFilterByid
      x-api-path-slug: apilistgroupsfiltersid-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Groups
      - List
      - Filter
      - As
      - Deleted
  /api/list/groupinterests/filters/{id}:
    delete:
      summary: Marks Groups List Filter as deleted
      description: Marks groups list filter as deleted.
      operationId: List_DeleteGroupInterestListFilterByid
      x-api-path-slug: apilistgroupinterestsfiltersid-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Groups
      - List
      - Filter
      - As
      - Deleted
  /api/list/todos/filters/{id}:
    delete:
      summary: Marks Todo List Filter as deleted
      description: Marks todo list filter as deleted.
      operationId: List_DeleteTodoListFilterByid
      x-api-path-slug: apilisttodosfiltersid-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Todo
      - List
      - Filter
      - As
      - Deleted
  /api/list/todotasks/filters/{id}:
    delete:
      summary: Marks Todos task List Filter as deleted
      description: Marks todos task list filter as deleted.
      operationId: List_DeleteTodoTaskListFilterByid
      x-api-path-slug: apilisttodotasksfiltersid-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Todos
      - Task
      - List
      - Filter
      - As
      - Deleted
  /api/list/followups/savefilter:
    put:
      summary: Save follow up filter
      description: Save follow up filter.
      operationId: List_SaveFollowUpFilterByfilter
      x-api-path-slug: apilistfollowupssavefilter-put
      parameters:
      - in: body
        name: filter
        description: Filter to save
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Save
      - Follow
      - Up
      - Filter
  /api/list/followups/filters/{id}:
    delete:
      summary: Marks Follow Up List Filter as deleted
      description: Marks follow up list filter as deleted.
      operationId: List_DeleteFollowUpListFilterByid
      x-api-path-slug: apilistfollowupsfiltersid-delete
      parameters:
      - in: path
        name: id
        description: Id of filter to delete
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Follow
      - Up
      - List
      - Filter
      - As
      - Deleted
  /api/list/feedback/followups/savefilter:
    put:
      summary: Save feedback follow up filter
      description: Save feedback follow up filter.
      operationId: List_SaveFeedbackFollowUpFilterByfilter
      x-api-path-slug: apilistfeedbackfollowupssavefilter-put
      parameters:
      - in: body
        name: filter
        description: Filter to save
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Save
      - Feedback
      - Follow
      - Up
      - Filter
  /api/list/feedbackfollowups/filters/{id}:
    delete:
      summary: Marks Feedback Follow Up List Filter as deleted
      description: Marks feedback follow up list filter as deleted.
      operationId: List_DeleteFeedbackFollowUpListFilterByid
      x-api-path-slug: apilistfeedbackfollowupsfiltersid-delete
      parameters:
      - in: path
        name: id
        description: Id of filter to delete
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Feedback
      - Follow
      - Up
      - List
      - Filter
      - As
      - Deleted
  /api/documentgeneration/multipropertymatch:
    post:
      summary: Generates a correspondence to multiple applicants, sending them a filtered
        set of the matching property roles
      description: Generates a correspondence to multiple applicants, sending them
        a filtered set of the matching property roles.
      operationId: DocumentGeneration_SendAutoMatchedPropertiesToApplicantListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationmultipropertymatch-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Multiple
      - Applicants
      - ""
      - Sending
      - Them
      - Filtered
      - Set
      - Of
      - Matching
      - Property
      - Roles
  /api/documentgeneration/multilettingspropertymatch:
    post:
      summary: Generates a correspondence to multiple letting applicants, sending
        them a filtered set of the matching letting property roles
      description: Generates a correspondence to multiple letting applicants, sending
        them a filtered set of the matching letting property roles.
      operationId: DocumentGeneration_SendAutoMatchedLettingsPropertiesToApplicantListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationmultilettingspropertymatch-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Multiple
      - Letting
      - Applicants
      - ""
      - Sending
      - Them
      - Filtered
      - Set
      - Of
      - Matching
      - Letting
      - Property
      - Roles
  /api/invoice/find:
    post:
      summary: Get filtered list of invoices
      description: Get filtered list of invoices.
      operationId: Invoice_GetInvoicesByfilterBypageSizeBypageNumber
      x-api-path-slug: apiinvoicefind-post
      parameters:
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Filtered
      - List
      - Of
      - Invoices
  /api/invoice/totals:
    post:
      summary: Get filtered list of invoices
      description: Get filtered list of invoices.
      operationId: Invoice_InvoiceTotalsByfilter
      x-api-path-slug: apiinvoicetotals-post
      parameters:
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Filtered
      - List
      - Of
      - Invoices
  /api/list/listsearchschema:
    get:
      summary: <param name="filterName">Filter for follow ups</param>
      description: <param name="filtername">filter for follow ups</param>.
      operationId: List_GetListSearchSchemaByfilterName
      x-api-path-slug: apilistlistsearchschema-get
      parameters:
      - in: query
        name: filterName
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - <param
      - Name=filterName>Filterfollow
      - Ups<
      - Param>
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