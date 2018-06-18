---
name: Oxford Dictionaries
x-slug: oxford-dictionaries
description: If you&rsquo;re looking to enhance your app or website with dictionary
  data, don&rsquo;t compromise on quality. The Oxford Dictionaries API offers easy
  and intuitive access to Oxfords dictionary content, which is trusted around the
  world. Here at Oxford Dictionaries, home of the OED, we love words. That&rsquo;s
  why we have experienced lexicographers tracking the living language, delving deep
  into our corpora and monitoring a wide range of media in order to understand how
  words are being used and how language is evolving. This research is used by our
  editors to write and edit dictionary entries and translations, meaning we&rsquo;re
  able to offer up-to-date, accurate, and reliable lexical content in multiple languages.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/oxford-dictionaries-api.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Filters
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/oxford-dictionaries/apis.md
specificationVersion: "0.14"
apis:
- name: Oxford Dictionaries Apply filters to response
  x-api-slug: oxford-dictionaries
  description: Use filters to limit the [entry](documentation/glossary?term=entry)
    information that is returned. For example, you may only require definitions and
    not everything else, or just [pronunciations](documentation/glossary?term=pronunciation).
    The full list of filters can be retrieved from the filters Utility endpoint. You
    can also specify values within the filter using '='. For example 'grammaticalFeatures=singular'.
    Filters can also be combined using a semicolon.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/oxford-dictionaries-api.png
  humanURL: https://developer.oxforddictionaries.com/
  baseURL: https://od-api-demo.oxforddictionaries.com:443//api/v1//entries/{source_lang}/{word_id}/{filters}
  tags: Entries,Source,Lang,Word,Id,Filters
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/oxford-dictionaries/entriessource-langword-idfilters-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/oxford-dictionaries/entriessource-langword-idfilters-get-openapi.md
- name: Oxford Dictionaries Lists available filters
  x-api-slug: oxford-dictionaries
  description: Returns a list of all the valid filters to construct API calls.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/oxford-dictionaries-api.png
  humanURL: https://developer.oxforddictionaries.com/
  baseURL: https://od-api-demo.oxforddictionaries.com:443//api/v1//filters
  tags: Filters
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/oxford-dictionaries/filters-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/oxford-dictionaries/filters-get-openapi.md
- name: Oxford Dictionaries Lists available filters for specific endpoint
  x-api-slug: oxford-dictionaries
  description: Returns a list of all the valid filters for a given endpoint to construct
    API calls.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/oxford-dictionaries-api.png
  humanURL: https://developer.oxforddictionaries.com/
  baseURL: https://od-api-demo.oxforddictionaries.com:443//api/v1//filters/{endpoint}
  tags: Filters,Endpoint
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/oxford-dictionaries/filtersendpoint-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/oxford-dictionaries/filtersendpoint-get-openapi.md
- name: Oxford Dictionaries Apply optional filters to Lemmatron response
  x-api-slug: oxford-dictionaries
  description: Retrieve available [lemmas](documentation/glossary?term=lemma) for
    a given [inflected](documentation/glossary?term=inflection) wordform. Filter results
    by categories.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/oxford-dictionaries-api.png
  humanURL: https://developer.oxforddictionaries.com/
  baseURL: https://od-api-demo.oxforddictionaries.com:443//api/v1//inflections/{source_lang}/{word_id}/{filters}
  tags: Inflections,Source,Lang,Word,Id,Filters
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/oxford-dictionaries/inflectionssource-langword-idfilters-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/oxford-dictionaries/inflectionssource-langword-idfilters-get-openapi.md
- name: Oxford Dictionaries Retrieve list of words for category with advanced options
  x-api-slug: oxford-dictionaries
  description: Use this to apply more complex filters to the [list of words](documentation/glossary?term=wordlist).
    For example, you may only want to filter out words for which all [senses](documentation/glossary?term=sense)
    match the filter, or only its 'prime sense'. You can also filter by word length
    or match by substring (prefix).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/oxford-dictionaries-api.png
  humanURL: https://developer.oxforddictionaries.com/
  baseURL: https://od-api-demo.oxforddictionaries.com:443//api/v1//wordlist/{source_lang}/{filters_advanced}
  tags: Wordlist,Source,Lang,Filters,Advanced
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/oxford-dictionaries/wordlistsource-langfilters-advanced-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/oxford-dictionaries/wordlistsource-langfilters-advanced-get-openapi.md
- name: Oxford Dictionaries Retrieve a list of words in a category
  x-api-slug: oxford-dictionaries
  description: Use this to retrieve a [list of words](documentation/glossary?term=wordlist)
    for particular [domain](documentation/glossary?term=domain), [lexical category](documentation/glossary?term=lexicalcategory),
    [register](documentation/glossary?term=registers) and/or [region](documentation/glossary?term=regions).
    View the full list of possible filters using the filters Utility endpoint.  The
    response only includes [headwords](documentation/glossary?term=headword), not
    all their possible [inflections](documentation/glossary?term=inflection). If you
    require a full [wordlist](documentation/glossary?term=wordlist) including [inflected
    forms](documentation/glossary?term=inflection), contact us and we can help.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/oxford-dictionaries-api.png
  humanURL: https://developer.oxforddictionaries.com/
  baseURL: https://od-api-demo.oxforddictionaries.com:443//api/v1//wordlist/{source_lang}/{filters_basic}
  tags: Wordlist,Source,Lang,Filters,Basic
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/oxford-dictionaries/wordlistsource-langfilters-basic-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/oxford-dictionaries/wordlistsource-langfilters-basic-get-openapi.md
- name: Oxford Dictionaries
  x-api-slug: oxford-dictionaries
  description: If you&rsquo;re looking to enhance your app or website with dictionary
    data, don&rsquo;t compromise on quality. The Oxford Dictionaries API offers easy
    and intuitive access to Oxfords dictionary content, which is trusted around the
    world. Here at Oxford Dictionaries, home of the OED, we love words. That&rsquo;s
    why we have experienced lexicographers tracking the living language, delving deep
    into our corpora and monitoring a wide range of media in order to understand how
    words are being used and how language is evolving. This research is used by our
    editors to write and edit dictionary entries and translations, meaning we&rsquo;re
    able to offer up-to-date, accurate, and reliable lexical content in multiple languages.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/oxford-dictionaries-api.png
  humanURL: https://developer.oxforddictionaries.com/
  baseURL: https://od-api-demo.oxforddictionaries.com:443//api/v1
  tags: Filters
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/filters/master/_listings/oxford-dictionaries/openapi.md
x-common:
- type: x-blog
  url: https://api-blog.oxforddictionaries.com/
- type: x-developer
  url: https://developer.oxforddictionaries.com/
- type: x-faq
  url: https://developer.oxforddictionaries.com/faq
- type: x-forum
  url: https://forum.oxforddictionaries.com/api/
- type: x-twitter
  url: https://twitter.com/OxfordWordsAPI
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---