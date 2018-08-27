swagger: "2.0"
x-collection-name: OpenRouteService
x-complete: 1
info:
  title: AP Metadata Services
  description: add-value-to-your-news-content-with-apu2019s-industryleading-metadata--accurate-comprehensive-richly-detailed-data-designed-specifically-for-use-by-news-publishers--ap-metadata-services-is-a-new-set-of-apis-that-gives-you-direct-access-to-the-same-metadata-system-that-supports-apu2019s-awardwinning-global-news-operation-
  version: v1
host: cv.ap.org
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  api/cm/:
    get:
      summary: Change Log
      description: Returns a list of changes to the AP vocabulary terms according
        to the specified criteria.
      operationId: getApiCm
      x-api-path-slug: apicm-get
      parameters:
      - in: query
        name: apiKey
        description: API Key
      - in: query
        name: authority
        description: authority
      - in: query
        name: enddate
        description: This parameter can be used in conjunction with the startdate
          parameter to  specify a date range
      - in: query
        name: format
        description: 'Specifies the output format: comma-separated values (CSV) or
          XML'
      - in: query
        name: lastversion
        description: Returns all change logs since (but not including) the specified
          version  number, in the format {AuthorityVersion}
      - in: query
        name: startdate
        description: eturns all change logs since (and including) the specified date
      - in: query
        name: version
        description: Returns the change log for the specified version number, in the
          format  {AuthorityVersion}
      responses:
        200:
          description: OK
      tags:
      - Change
      - Log