---
swagger: "2.0"
x-collection-name: Trello
x-complete: 0
info:
  title: Trello Get Lists List Cards Filter
  description: Get lists list cards filter.
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /boards/{idBoard}/cards/{filter}:
    get:
      summary: Get Boards Cards Filter
      description: Get boards cards filter.
      operationId: getBoardsCardsByIdBoardByFilter
      x-api-path-slug: boardsidboardcardsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Cards
      - Filter
  /boards/{idBoard}/lists/{filter}:
    get:
      summary: Get Boards Lists Filter
      description: Get boards lists filter.
      operationId: getBoardsListsByIdBoardByFilter
      x-api-path-slug: boardsidboardlistsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Lists
      - Filter
  /boards/{idBoard}/members/{filter}:
    get:
      summary: Get Boards Members Filter
      description: Get boards members filter.
      operationId: getBoardsMembersByIdBoardByFilter
      x-api-path-slug: boardsidboardmembersfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Members
      - Filter
  /checklists/{idChecklist}/cards/{filter}:
    get:
      summary: Get Checklists Cards Filter
      description: Get checklists cards filter.
      operationId: getChecklistsCardsByIdChecklistByFilter
      x-api-path-slug: checklistsidchecklistcardsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idChecklist
        description: idChecklist
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Checklists
      - Cards
      - Filter
  /lists/{idList}/cards/{filter}:
    get:
      summary: Get Lists List Cards Filter
      description: Get lists list cards filter.
      operationId: getListsCardsByIdListByFilter
      x-api-path-slug: listsidlistcardsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idList
        description: idList
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
      - Cards
      - Filter
  /members/{idMember}/boards/{filter}:
    get:
      summary: Get Members Boards Filter
      description: Get members boards filter.
      operationId: getMembersBoardsByIdMemberByFilter
      x-api-path-slug: membersidmemberboardsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boards
      - Filter
  /members/{idMember}/cards/{filter}:
    get:
      summary: Get Members Cards Filter
      description: Get members cards filter.
      operationId: getMembersCardsByIdMemberByFilter
      x-api-path-slug: membersidmembercardsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Cards
      - Filter
  /members/{idMember}/notifications/{filter}:
    get:
      summary: Get Members Notifications Filter
      description: Get members notifications filter.
      operationId: getMembersNotificationsByIdMemberByFilter
      x-api-path-slug: membersidmembernotificationsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Notifications
      - Filter
  /members/{idMember}/organizations/{filter}:
    get:
      summary: Get Members Organizations Filter
      description: Get members organizations filter.
      operationId: getMembersOrganizationsByIdMemberByFilter
      x-api-path-slug: membersidmemberorganizationsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Organizations
      - Filter
  /organizations/{idOrg}/boards/{filter}:
    get:
      summary: Get Organizations Boards Filter
      description: Get organizations boards filter.
      operationId: getOrganizationsBoardsByIdOrgByFilter
      x-api-path-slug: organizationsidorgboardsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Boards
      - Filter
  /organizations/{idOrg}/members/{filter}:
    get:
      summary: Get Organizations Members Filter
      description: Get organizations members filter.
      operationId: getOrganizationsMembersByIdOrgByFilter
      x-api-path-slug: organizationsidorgmembersfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Members
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