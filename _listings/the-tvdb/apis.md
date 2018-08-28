---
name: The TVDB
x-slug: the-tvdb
description: TheTVDB.com is a community driven database of television shows. All content
  and images on the site have been contributed by the sites users; the site uses moderated
  editing to maintain its own standards. The database schema and website are open
  source under the GNU General Public License.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
x-kinRank: "7"
x-alexaRank: "0"
tags: Episodes
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/the-tvdb/apis.md
specificationVersion: "0.14"
apis:
- name: The TVDB API v2 - Get Episodes
  x-api-slug: episodesid-get
  description: Returns the full information for a given episode id. __Deprecation
    Warning:__ The _director_ key will be deprecated in favor of the new _directors_
    key in a future release.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/the-tvdb/episodesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/the-tvdb/episodesid-get-openapi.md
- name: The TVDB API v2 - Get Series Episodes
  x-api-slug: seriesidepisodes-get
  description: All episodes for a given series. Paginated with 100 results per page.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/the-tvdb/seriesidepisodes-get-openapi.md
- name: The TVDB API v2 - Get Series Episodes Query
  x-api-slug: seriesidepisodesquery-get
  description: This route allows the user to query against episodes for the given
    series. The response is a paginated array of episode records that have been filtered
    down to basic information.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/the-tvdb/seriesidepisodesquery-get-openapi.md
- name: The TVDB API v2 - Get Series Episodes Query Params
  x-api-slug: seriesidepisodesqueryparams-get
  description: Returns the allowed query keys for the `/series/{id}/episodes/query`
    route
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/the-tvdb/seriesidepisodesqueryparams-get-openapi.md
- name: The TVDB API v2 - Get Series Episodes Summary
  x-api-slug: seriesidepisodessummary-get
  description: |-
    Returns a summary of the episodes and seasons available for the series.

    __Note__: Season "0" is for all episodes that are considered to be specials.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/the-tvdb/seriesidepisodessummary-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://the.open.movie.database.api.gallery.streamdata.io
- type: x-api-stack
  url: http://the.tvdb.stack.network
- type: x-documentation
  url: https://api.thetvdb.com/swagger
- type: x-website
  url: http://thetvdb.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---