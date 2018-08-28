swagger: "2.0"
x-collection-name: Botify
x-complete: 1
info:
  title: Botify
  description: botify-saas-api
  version: 1.0.0
host: api.botify.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /analyses/{username}/{project_slug}/{analysis_slug}/urls/suggested_filters:
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Urls Suggested
        Filters
      description: Parameters analyses username project slug analysis slug urls suggested
        filters.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugUrlsSuggestedFilters
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlssuggested-filters-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Suggested
      - Filters
    post:
      summary: Post Analyses Username Project Slug Analysis Slug Urls Suggested Filters
      description: Return most frequent segments (= suggested patterns in the previous
        version) for a Botify Query.
      operationId: postAnalysesUsernameProjectSlugAnalysisSlugUrlsSuggestedFilters
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlssuggested-filters-post
      parameters:
      - in: query
        name: area
        description: Analysis context
      - in: body
        name: UrlsAggsQuery
        description: UrlsAggs query
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Suggested
      - Filters
  /projects/{username}/{project_slug}/filters:
    get:
      summary: Get Projects Username Project Slug Filters
      description: List all the project's saved filters (each filter's name, ID and
        filter value)
      operationId: getProjectsUsernameProjectSlugFilters
      x-api-path-slug: projectsusernameproject-slugfilters-get
      parameters:
      - in: query
        name: page
        description: Page Number
      - in: query
        name: size
        description: Page Size
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Username
      - Project
      - Slug
      - Filters
    parameters:
      summary: Parameters Projects Username Project Slug Filters
      description: Parameters projects username project slug filters.
      operationId: parametersProjectsUsernameProjectSlugFilters
      x-api-path-slug: projectsusernameproject-slugfilters-parameters
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Username
      - Project
      - Slug
      - Filters
  /projects/{username}/{project_slug}/filters/{identifier}:
    get:
      summary: Get Projects Username Project Slug Filters Entifier
      description: Retrieves a specific saved filter's name, ID and filter value
      operationId: getProjectsUsernameProjectSlugFiltersEntifier
      x-api-path-slug: projectsusernameproject-slugfiltersidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Username
      - Project
      - Slug
      - Filters
      - Identifier
    parameters:
      summary: Parameters Projects Username Project Slug Filters Entifier
      description: Parameters projects username project slug filters entifier.
      operationId: parametersProjectsUsernameProjectSlugFiltersEntifier
      x-api-path-slug: projectsusernameproject-slugfiltersidentifier-parameters
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Username
      - Project
      - Slug
      - Filters
      - Identifier