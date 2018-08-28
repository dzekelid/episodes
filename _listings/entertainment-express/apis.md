---
name: Entertainment Express
x-slug: entertainment-express
description: Internet Video Archive (IVA) is a leading entertainment data company
  providing metadata, images and trailers/clips, for movie and TV content. With the
  launch of its award-winning Entertainment Express APIs, clients can easily access
  everything they need to create engaging content discovery experiences. By using
  Entertainment Express, clients can also connect to other services like movie showtimes
  and ticketing, content recommendations, content availability and TV channel line-ups.
  With over a million titles, episodes and over 150,000 videos available, IVA makes
  it easy for developers to integrate all the services they need at a very affordable
  price.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Episodes
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/apis.md
specificationVersion: "0.14"
apis:
- name: Entertainment Express - Returns list of unique EpisodeId changes greater than
    or equal to date (UTC)
  x-api-slug: changesepisodeshistory-get
  description: For each updated episode ID, pull the full episode data for that ID
    and update.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/changesepisodeshistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/changesepisodeshistory-get-openapi.md
- name: Entertainment Express - Returns list of unique EpisodeId and Entity changes
    greater than or equal to date (UTC).
  x-api-slug: changesepisodeshistorywithentity-get
  description: Lists each episode ID that has changed as well as the entity in the
    object that changed.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/changesepisodeshistorywithentity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/changesepisodeshistorywithentity-get-openapi.md
- name: Entertainment Express - Get GoWatchIt Episode Availability.
  x-api-slug: gowatchitepisodesidavailabilities-get
  description: Returns GoWatchit episode availability by Entertainment Episode ID.
    Special permission is required to access this endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/gowatchitepisodesidavailabilities-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/gowatchitepisodesidavailabilities-get-openapi.md
- name: Entertainment Express - Returns an Episode object for a requested Episode
    ID.
  x-api-slug: showsseasonsepisodesid-get
  description: Returns the episode details for a specific episode ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/showsseasonsepisodesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/showsseasonsepisodesid-get-openapi.md
- name: Entertainment Express - Get Episode by ShowId, Season Number and Episode Number.
  x-api-slug: showsidseasonsseasonnumberepisodesepisodenumber-get
  description: Requires a valid ShowId, Season Number and Episode Number.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/showsidseasonsseasonnumberepisodesepisodenumber-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/showsidseasonsseasonnumberepisodesepisodenumber-get-openapi.md
- name: Entertainment Express - Get Episode by ShowId, Season Number and Episode Number.
  x-api-slug: showsseasonsepisode-get
  description: Some use cases find it useful to be able to pass a season number and
    episode number of a known show to get the data for that exact episode.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/showsseasonsepisode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/showsseasonsepisode-get-openapi.md
- name: Entertainment Express - Get Episode by ShowId, Season Number and Episode Number.
  x-api-slug: showsidseasonsseasonnumberepisodesepisodenumber-get
  description: Requires a valid ShowId, Season Number and Episode Number.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/showsidseasonsseasonnumberepisodesepisodenumber-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/showsidseasonsseasonnumberepisodesepisodenumber-get-openapi.md
- name: Entertainment Express - Get Episode by ShowId, Season Number and Episode Number.
  x-api-slug: showsseasonsepisode-get
  description: Some use cases find it useful to be able to pass a season number and
    episode number of a known show to get the data for that exact episode.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/showsseasonsepisode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/showsseasonsepisode-get-openapi.md
- name: Entertainment Express - Get Episode by ShowId, Season Number and Episode Number.
  x-api-slug: showsidseasonsseasonnumberepisodesepisodenumber-get
  description: Requires a valid ShowId, Season Number and Episode Number.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/showsidseasonsseasonnumberepisodesepisodenumber-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/showsidseasonsseasonnumberepisodesepisodenumber-get-openapi.md
- name: Entertainment Express - Get Episode by ShowId, Season Number and Episode Number.
  x-api-slug: showsseasonsepisode-get
  description: Some use cases find it useful to be able to pass a season number and
    episode number of a known show to get the data for that exact episode.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/showsseasonsepisode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/showsseasonsepisode-get-openapi.md
- name: Entertainment Express - Get Episode by ShowId, Season Number and Episode Number.
  x-api-slug: showsidseasonsseasonnumberepisodesepisodenumber-get
  description: Requires a valid ShowId, Season Number and Episode Number.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/showsidseasonsseasonnumberepisodesepisodenumber-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/episodes/master/_listings/entertainment-express/showsidseasonsseasonnumberepisodesepisodenumber-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://emuseum.api.docs.api.gallery.streamdata.io
- type: x-api-stack
  url: http://entertainment.express.stack.network
- type: x-blog
  url: https://www.internetvideoarchive.com/blog/
- type: x-developer
  url: https://developer.iva-api.com/
- type: x-pricing
  url: https://www.internetvideoarchive.com/pricing/
- type: x-website
  url: https://www.internetvideoarchive.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---