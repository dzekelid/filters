---
swagger: "2.0"
x-collection-name: Oxford Dictionaries
x-complete: 0
info:
  title: Oxford Dictionaries Retrieve a list of words in a category
  description: Use this to retrieve a [list of words](documentation/glossary?term=wordlist)
    for particular [domain](documentation/glossary?term=domain), [lexical category](documentation/glossary?term=lexicalcategory),
    [register](documentation/glossary?term=registers) and/or [region](documentation/glossary?term=regions).
    View the full list of possible filters using the filters Utility endpoint.  The
    response only includes [headwords](documentation/glossary?term=headword), not
    all their possible [inflections](documentation/glossary?term=inflection). If you
    require a full [wordlist](documentation/glossary?term=wordlist) including [inflected
    forms](documentation/glossary?term=inflection), contact us and we can help.
  termsOfService: http://helloreverb.com/terms/
  version: 1.8.0
host: od-api-demo.oxforddictionaries.com:443
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /entries/{source_lang}/{word_id}/{filters}:
    get:
      summary: Apply filters to response
      description: Use filters to limit the [entry](documentation/glossary?term=entry)
        information that is returned. For example, you may only require definitions
        and not everything else, or just [pronunciations](documentation/glossary?term=pronunciation).
        The full list of filters can be retrieved from the filters Utility endpoint.
        You can also specify values within the filter using '='. For example 'grammaticalFeatures=singular'.
        Filters can also be combined using a semicolon.
      operationId: getEntriesSourceLangWordFilters
      x-api-path-slug: entriessource-langword-idfilters-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Entries
      - Source
      - Lang
      - Word
      - Id
      - Filters
  /filters:
    get:
      summary: Lists available filters
      description: Returns a list of all the valid filters to construct API calls.
      operationId: getFilters
      x-api-path-slug: filters-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Filters
  /filters/{endpoint}:
    get:
      summary: Lists available filters for specific endpoint
      description: Returns a list of all the valid filters for a given endpoint to
        construct API calls.
      operationId: getFiltersEndpoint
      x-api-path-slug: filtersendpoint-get
      parameters:
      - in: path
        name: endpoint
        description: Name of the endpoint
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Filters
      - Endpoint
  /inflections/{source_lang}/{word_id}/{filters}:
    get:
      summary: Apply optional filters to Lemmatron response
      description: Retrieve available [lemmas](documentation/glossary?term=lemma)
        for a given [inflected](documentation/glossary?term=inflection) wordform.
        Filter results by categories.
      operationId: getInflectionsSourceLangWordFilters
      x-api-path-slug: inflectionssource-langword-idfilters-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: word_id
        description: The input word
      responses:
        200:
          description: OK
      tags:
      - Inflections
      - Source
      - Lang
      - Word
      - Id
      - Filters
  /wordlist/{source_lang}/{filters_advanced}:
    get:
      summary: Retrieve list of words for category with advanced options
      description: Use this to apply more complex filters to the [list of words](documentation/glossary?term=wordlist).
        For example, you may only want to filter out words for which all [senses](documentation/glossary?term=sense)
        match the filter, or only its 'prime sense'. You can also filter by word length
        or match by substring (prefix).
      operationId: getWordlistSourceLangFiltersAdvanced
      x-api-path-slug: wordlistsource-langfilters-advanced-get
      parameters:
      - in: query
        name: exact
        description: If exact=true wordlist returns a list of entries that exactly
          matches the search string
      - in: query
        name: exclude
        description: Semicolon separated list of parameters-value pairs (same as filters)
      - in: query
        name: exclude_prime_senses
        description: Semicolon separated list of parameters-value pairs (same as filters)
      - in: query
        name: exclude_senses
        description: Semicolon separated list of parameters-value pairs (same as filters)
      - in: path
        name: filters_advanced
        description: 'Semicolon separated list of wordlist parameters, presented as
          value pairs: LexicalCategory, domains, regions, registers'
      - in: query
        name: limit
        description: Limit the number of results per response
      - in: query
        name: No Name
      - in: query
        name: offset
        description: Offset the start number of the result
      - in: query
        name: prefix
        description: Filter words that start with prefix parameter
      - in: query
        name: word_length
        description: Parameter to speficy the minimum (>), exact or maximum (5 - more
          than 5 chars; 5
      responses:
        200:
          description: OK
      tags:
      - Wordlist
      - Source
      - Lang
      - Filters
      - Advanced
  /wordlist/{source_lang}/{filters_basic}:
    get:
      summary: Retrieve a list of words in a category
      description: Use this to retrieve a [list of words](documentation/glossary?term=wordlist)
        for particular [domain](documentation/glossary?term=domain), [lexical category](documentation/glossary?term=lexicalcategory),
        [register](documentation/glossary?term=registers) and/or [region](documentation/glossary?term=regions).
        View the full list of possible filters using the filters Utility endpoint.  The
        response only includes [headwords](documentation/glossary?term=headword),
        not all their possible [inflections](documentation/glossary?term=inflection).
        If you require a full [wordlist](documentation/glossary?term=wordlist) including
        [inflected forms](documentation/glossary?term=inflection), contact us and
        we can help.
      operationId: getWordlistSourceLangFiltersBasic
      x-api-path-slug: wordlistsource-langfilters-basic-get
      parameters:
      - in: path
        name: filters_basic
        description: 'Semicolon separated list of wordlist parameters, presented as
          value pairs: LexicalCategory, domains, regions, registers'
      - in: query
        name: limit
        description: Limit the number of results per response
      - in: query
        name: No Name
      - in: query
        name: offset
        description: Offset the start number of the result
      responses:
        200:
          description: OK
      tags:
      - Wordlist
      - Source
      - Lang
      - Filters
      - Basic
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