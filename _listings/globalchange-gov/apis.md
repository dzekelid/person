---
name: GlobalChange.gov
x-slug: globalchange-gov
description: The U.S. Global Change Research Program (USGCRP) was established by Presidential
  Initiative in 1989 and mandated by Congress in the Global Change Research Act (GCRA)
  of 1990 to &ldquo;assist the Nation and the world to understand, assess, predict,
  and respond to human-induced and natural processes of global change.&rdquo;
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/global-change-gov.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Person
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/person/master/_listings/globalchange-gov/apis.md
specificationVersion: "0.14"
apis:
- name: Global Change Information System API - Redirect to a person based on a name
  x-api-slug: personname-get
  description: Given a name (case sensitive, concatenated by dashes), redirect if
    there is a single match.  The first and last names can be in either order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/global-change-gov.png
  humanURL: http://globalchange.gov/
  baseURL: https://data.globalchange.gov//
  tags: Federal Government, Federal Government, Stack Network, API Provider, Profiles,
    General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/person/master/_listings/globalchange-gov/personname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/person/master/_listings/globalchange-gov/personname-get-openapi.md
- name: Global Change Information System API - Redirect to a person based on an ORCID.
  x-api-slug: personorcid-get
  description: Given an ORCID, if there is a match, redirect to the persons URI.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/global-change-gov.png
  humanURL: http://globalchange.gov/
  baseURL: https://data.globalchange.gov//
  tags: Federal Government, Federal Government, Stack Network, API Provider, Profiles,
    General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/person/master/_listings/globalchange-gov/personorcid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/person/master/_listings/globalchange-gov/personorcid-get-openapi.md
- name: Global Change Information System API - Get a representation of a person.
  x-api-slug: personperson-identifier-get
  description: Get JSON which represents the structure of a person.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/global-change-gov.png
  humanURL: http://globalchange.gov/
  baseURL: https://data.globalchange.gov//
  tags: Federal Government, Federal Government, Stack Network, API Provider, Profiles,
    General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/person/master/_listings/globalchange-gov/personperson-identifier-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/person/master/_listings/globalchange-gov/personperson-identifier-get-openapi.md
- name: Global Change Information System API - Show contributions of a certain type
    by a person
  x-api-slug: personperson-identifiercontributionsrole-type-identifierresource-get
  description: Given a resource (dataset, report, etc.) and a role (editor, etc),
    and an identifier for a person, show the resources to which the person has contributed
    in that role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/global-change-gov.png
  humanURL: http://globalchange.gov/
  baseURL: https://data.globalchange.gov//
  tags: Federal Government, Federal Government, Stack Network, API Provider, Profiles,
    General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/person/master/_listings/globalchange-gov/personperson-identifiercontributionsrole-type-identifierresource-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/person/master/_listings/globalchange-gov/personperson-identifiercontributionsrole-type-identifierresource-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://gitter.api.gallery.streamdata.io
- type: x-api-stack
  url: http://globalchange.gov.stack.network
- type: x-developer
  url: http://data.globalchange.gov/
- type: x-website
  url: http://globalchange.gov/
- type: x-website
  url: http://globalchange.gov
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---