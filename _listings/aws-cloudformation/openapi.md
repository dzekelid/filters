swagger: "2.0"
x-collection-name: AWS CloudFormation
x-complete: 1
info:
  title: AWS CloudFormation API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListStacks:
    get:
      summary: List Stacks
      description: Returns the summary information for stacks whose status matches
        the specified StackStatusFilter.
      operationId: listStacks
      x-api-path-slug: actionliststacks-get
      parameters:
      - in: query
        name: NextToken
        description: A string that identifies the next page of stacks that you want
          to retrieve
        type: string
      - in: query
        name: StackStatusFilter.member.N
        description: Stack status to use as a filter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stacks