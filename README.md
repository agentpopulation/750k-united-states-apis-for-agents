<p align="center"><img src="assets/banner.svg" width="100%" alt="United States API endpoints: 751,070 API endpoints passed a keyless data call"></p>

# 🇺🇸 United States API endpoints

**751,070 API endpoints filed under country code US that answered a keyless GET with a data body. For agent and app builders.**

<p align="center"><a href="#files"><img src="https://img.shields.io/badge/endpoints-751%2C070-6366F1" alt="endpoints: 751,070"></a> <a href="#columns-and-tags"><img src="https://img.shields.io/badge/keyless%20JSON-751%2C069-6366F1" alt="keyless JSON: 751,069"></a> <a href="#whats-inside"><img src="https://img.shields.io/badge/services-23%2C179-0F172A" alt="services: 23,179"></a> <a href="#whats-inside"><img src="https://img.shields.io/badge/country-US-EA580C" alt="country: US"></a> <a href="LICENSE"><img src="https://img.shields.io/badge/licence-CC%20BY%204.0-0F172A" alt="licence: CC BY 4.0"></a></p>

<p align="center"><a href="#whats-in-it-for-you">What's in it</a> · <a href="#for-ai-agents">For AI agents</a> · <a href="#quick-start">Quick start</a> · <a href="#test-it-yourself">Test it yourself</a> · <a href="#files">Files</a> · <a href="#licence-and-credit">Licence</a> · <a href="#part-of-10m-api-endpoints-for-ai-agents">More packs</a></p>

This repository holds a 1,000-row sample and the services list; the full list of 751,070 endpoints is one download from the [latest release](https://github.com/agentpopulation/750k-united-states-apis-for-agents/releases/latest).

**Endpoints filed under country code US, for building an agent or app for the United States.** Map-layer queries from counties, cities, state agencies, regional commissions and nonprofits (parcels, hydrants, crash data, election results, habitat), as URLs that answered with no key on their test date.

Selection rule: rows where `country is US`, less the rows that a leave-out rule drops (each counted under Known limits).

385,317 of these 751,070 rows match the focus rule (below); the others are in the pack by the selection rule only, and Known limits says what they are. 739,487 rows (98.5%) are map layers on ArcGIS Online, where anyone can publish.

## In plain words

**What is an API endpoint?** An API endpoint is one web address that a program can ask for data, for example the latest reading at one weather station. A single service, such as a national weather agency, can have thousands of endpoints: one per station, city or dataset. This pack counts endpoints, not separate services.

**What does "passed a data call" mean?** On the date shown in each row, AgentPopulation sent one plain request to that address, with no password or key, and got a non-empty data body back (JSON, CSV, XML or a file): not an error page and not an empty result. Some bodies describe a dataset rather than hold its values; see Known limits. It shows the address answered with data on that day. It is not a promise that it answers today, and licences and usage limits were not reviewed.

## What's in it for you

Four ways to use this pack. Each bucket gives a count, a filter you can apply to the CSV, one example that passed, and a list of recommended starting points with the rule that picked them. Buckets overlap; a row can fit more than one.

Examples, recommended lists and the preview are drawn from rows that match this pack's focus rule, so a row that the selection rule put in this pack but that is about something else is not shown as a starting point. Counts cover the whole bucket.

<details>
<summary>The focus rule</summary>

Focus rule: `NOT title matches /(?<![a-z])(test|tests|testing|draft|drafts|copy|sample|samples|demo|untitled|scratch|temp|tmp|delete|deleteme|practice|dummy|example|training)(?![a-z])|final_final|\d{7,}/i AND (NOT url matches ///(services[0-9]*(-[a-z0-9]+)?|utility)\.arcgis\.com//i OR NOT service matches /^ArcGIS organization /i)`

</details>

### 🤖 Agent tools: Keyless JSON layers and tables an agent can call (United States)

**751,069** endpoints from 23,179 services · Wrap one layer query as a get_layer_features tool: pass a where clause or a bounding box, return the matching features with a timeout.

751,069 of these are map-layer queries that asked for a few records (`resultRecordCount`); add a where clause or a geometry to ask about one place, and page through for the whole layer.

Start with: `tags has agent-ready`

Example: [Áreas\_Eco\_Oro](https://services.arcgis.com/F7DSX1DSNSiWmOqh/ArcGIS/rest/services/%C3%81reas_Eco_Oro/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) · The Nature Conservancy (ArcGIS Online) · passed 2026-11-16

<details>
<summary>Recommended starting points: 8 services, picked by the stated criteria inside</summary>

**Recommended starting points.** Selected by stated criteria, not a ranking of quality: Services in this pack with the most endpoints that match this bucket and are tagged `agent-ready` (no key sent in the test call, JSON body, passed a data call). Ties go to the service with more country codes, then by name. Only services with at least one bucket row that matches the focus rule are listed, and the sample comes from those rows; the counts cover the whole bucket. The sample URL is the first row by URL sort after preferring, in this order: rows that match the bucket's sample preference when it has one, rows that return values rather than describe a dataset or a service (not ERDDAP /info/ pages, OGC GetCapabilities requests, bare OWS addresses, PxWeb tables, UN SDG series lists, Statistics Canada download pointers, WorldPop listings, GTFS validation reports, untitled rows or service root addresses), and agent-ready rows. Sample preference in this bucket: `url matches //query\?/i`. Services named "ArcGIS organization" hold map layers from many owners and are added only when fewer than 5 other services match.

| Service (host) | Endpoints in bucket | In pack | Country codes in bucket | Formats in bucket | Sample URL that passed |
|---|---:|---:|---|---|---|
| The Nature Conservancy (ArcGIS Online) (services.arcgis.com) | 3,303 | 3,303 | US | json | [Áreas\_Eco\_Oro](https://services.arcgis.com/F7DSX1DSNSiWmOqh/ArcGIS/rest/services/%C3%81reas_Eco_Oro/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| NOAA GeoPlatform (ArcGIS Online) (services2.arcgis.com) | 3,045 | 3,045 | US | json | [0Z\_850mbHeightsWinds](https://services2.arcgis.com/C8EMgrsFcRFL6LrL/ArcGIS/rest/services/0Z_850mbHeightsWinds/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Africa GeoPortal (ArcGIS Online) (services8.arcgis.com) | 2,938 | 2,938 | US | json | [électrique\_saly](https://services8.arcgis.com/oTalEaSXAuyNT7xf/ArcGIS/rest/services/%C3%A9lectrique_saly/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| FEMA AGOL (ArcGIS Online) (services.arcgis.com) | 2,706 | 2,706 | US | json | [02\_Structures\_Display](https://services.arcgis.com/XG15cJAlne2vxtgt/ArcGIS/rest/services/02_Structures_Display/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Georgia Association of Regional Commissions (ArcGIS Online) (services1.arcgis.com) | 2,703 | 2,703 | US | json | [2010\_Census\_Tracts\_with\_Disadvantaged\_C…](https://services1.arcgis.com/Ug5xGQbHsD8zuZzM/ArcGIS/rest/services/2010_Census_Tracts_with_Disadvantaged_Communities_Data/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| ArcGIS Online for Maryland (ArcGIS Online) (services.arcgis.com) | 2,537 | 2,537 | US | json | [12DigitPivotYearsData](https://services.arcgis.com/njFNhDsUCentVYJW/ArcGIS/rest/services/12DigitPivotYearsData/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| HNTB GeoShare (ArcGIS Online) (services.arcgis.com) | 2,457 | 2,457 | US | json | [1000\_FT\_Buffer\_SR70\_66](https://services.arcgis.com/rD2ylXRs80UroD90/ArcGIS/rest/services/1000_FT_Buffer_SR70_66/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| National Audubon Society (ArcGIS Online) (services1.arcgis.com) | 2,223 | 2,223 | US | json | [Áreas\_clave\_para\_la\_Biodiversidad\_KBA\_c…](https://services1.arcgis.com/lDFzr3JyGEn5Eymu/ArcGIS/rest/services/%C3%81reas_clave_para_la_Biodiversidad_KBA_con_estado_IBA_confirmado_Peru/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |

</details>

### 📱 App features: Map layers to draw in an app (United States)

**751,070** endpoints from 23,179 services · Add the layers to an app map: read the layer once for its fields, then ask for the features in the visible area.

Start with: `url matches //(Feature|Map)Server//i`

Example: [Áreas\_Eco\_Oro](https://services.arcgis.com/F7DSX1DSNSiWmOqh/ArcGIS/rest/services/%C3%81reas_Eco_Oro/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) · The Nature Conservancy (ArcGIS Online) · passed 2026-11-16

<details>
<summary>Recommended starting points: 8 services, picked by the stated criteria inside</summary>

**Recommended starting points.** Selected by stated criteria, not a ranking of quality: Services in this pack with the most endpoints that match this bucket and passed a data call. Ties go to the service with more country codes, then by name. Only services with at least one bucket row that matches the focus rule are listed, and the sample comes from those rows; the counts cover the whole bucket. The sample URL is the first row by URL sort after preferring, in this order: rows that match the bucket's sample preference when it has one, rows that return values rather than describe a dataset or a service (not ERDDAP /info/ pages, OGC GetCapabilities requests, bare OWS addresses, PxWeb tables, UN SDG series lists, Statistics Canada download pointers, WorldPop listings, GTFS validation reports, untitled rows or service root addresses), and agent-ready rows. Services named "ArcGIS organization" hold map layers from many owners and are added only when fewer than 5 other services match.

| Service (host) | Endpoints in bucket | In pack | Country codes in bucket | Formats in bucket | Sample URL that passed |
|---|---:|---:|---|---|---|
| The Nature Conservancy (ArcGIS Online) (services.arcgis.com) | 3,303 | 3,303 | US | json | [Áreas\_Eco\_Oro](https://services.arcgis.com/F7DSX1DSNSiWmOqh/ArcGIS/rest/services/%C3%81reas_Eco_Oro/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| NOAA GeoPlatform (ArcGIS Online) (services2.arcgis.com) | 3,045 | 3,045 | US | json | [0Z\_850mbHeightsWinds](https://services2.arcgis.com/C8EMgrsFcRFL6LrL/ArcGIS/rest/services/0Z_850mbHeightsWinds/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Africa GeoPortal (ArcGIS Online) (services8.arcgis.com) | 2,938 | 2,938 | US | json | [électrique\_saly](https://services8.arcgis.com/oTalEaSXAuyNT7xf/ArcGIS/rest/services/%C3%A9lectrique_saly/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| FEMA AGOL (ArcGIS Online) (services.arcgis.com) | 2,706 | 2,706 | US | json | [02\_Structures\_Display](https://services.arcgis.com/XG15cJAlne2vxtgt/ArcGIS/rest/services/02_Structures_Display/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Georgia Association of Regional Commissions (ArcGIS Online) (services1.arcgis.com) | 2,703 | 2,703 | US | json | [2010\_Census\_Tracts\_with\_Disadvantaged\_C…](https://services1.arcgis.com/Ug5xGQbHsD8zuZzM/ArcGIS/rest/services/2010_Census_Tracts_with_Disadvantaged_Communities_Data/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| ArcGIS Online for Maryland (ArcGIS Online) (services.arcgis.com) | 2,537 | 2,537 | US | json | [12DigitPivotYearsData](https://services.arcgis.com/njFNhDsUCentVYJW/ArcGIS/rest/services/12DigitPivotYearsData/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| HNTB GeoShare (ArcGIS Online) (services.arcgis.com) | 2,457 | 2,457 | US | json | [1000\_FT\_Buffer\_SR70\_66](https://services.arcgis.com/rD2ylXRs80UroD90/ArcGIS/rest/services/1000_FT_Buffer_SR70_66/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| National Audubon Society (ArcGIS Online) (services1.arcgis.com) | 2,223 | 2,223 | US | json | [Áreas\_clave\_para\_la\_Biodiversidad\_KBA\_c…](https://services1.arcgis.com/lDFzr3JyGEn5Eymu/ArcGIS/rest/services/%C3%81reas_clave_para_la_Biodiversidad_KBA_con_estado_IBA_confirmado_Peru/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |

</details>

### 🧠 Grounding and data pipelines: Statistics, boundaries, parcels and inventories for scheduled loads (United States)

**80,338** endpoints from 11,110 services · Load the tables and layers on a schedule into your own store, so an agent can cite a dated source.

Start with: `format in (csv, xml, geojson) OR title matches /statist|census|population|boundar|parcel|zoning|district|budget|election|crash|permit|inventory|land ?use|landuse|cadast|address/i`

Example: [2010\_Census\_Tracts\_with\_Disadvantaged\_Communities…](https://services1.arcgis.com/Ug5xGQbHsD8zuZzM/ArcGIS/rest/services/2010_Census_Tracts_with_Disadvantaged_Communities_Data/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) · Georgia Association of Regional Commissions (ArcGIS Online) · passed 2026-11-16

<details>
<summary>Recommended starting points: 8 services, picked by the stated criteria inside</summary>

**Recommended starting points.** Selected by stated criteria, not a ranking of quality: Services in this pack with the most endpoints that match this bucket and passed a data call. Ties go to the service with more country codes, then by name. Only services with at least one bucket row that matches the focus rule are listed, and the sample comes from those rows; the counts cover the whole bucket. The sample URL is the first row by URL sort after preferring, in this order: rows that match the bucket's sample preference when it has one, rows that return values rather than describe a dataset or a service (not ERDDAP /info/ pages, OGC GetCapabilities requests, bare OWS addresses, PxWeb tables, UN SDG series lists, Statistics Canada download pointers, WorldPop listings, GTFS validation reports, untitled rows or service root addresses), and agent-ready rows. Services named "ArcGIS organization" hold map layers from many owners and are added only when fewer than 5 other services match.

| Service (host) | Endpoints in bucket | In pack | Country codes in bucket | Formats in bucket | Sample URL that passed |
|---|---:|---:|---|---|---|
| Georgia Association of Regional Commissions (ArcGIS Online) (services1.arcgis.com) | 458 | 2,703 | US | json | [2010\_Census\_Tracts\_with\_Disadvantaged\_C…](https://services1.arcgis.com/Ug5xGQbHsD8zuZzM/ArcGIS/rest/services/2010_Census_Tracts_with_Disadvantaged_Communities_Data/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Office for National Statistics (ArcGIS Online) (services1.arcgis.com) | 396 | 676 | US | json | [Built-up Area (2011) to Local Authority…](https://services1.arcgis.com/ESMARspQHYMw9BZ9/arcgis/rest/services/BUA11_LAD11_EW_LU_ccfff9f71c3c48b9b49ecc9d0e79c8c8/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=5&f=json) (2026-11-16) |
| Esri (ArcGIS Online) (services.arcgis.com) | 388 | 681 | US | json | [ACS\_10\_14\_Children\_in\_Grandparent\_House…](https://services.arcgis.com/P3ePLMYs2RVChkJx/ArcGIS/rest/services/ACS_10_14_Children_in_Grandparent_Households_Boundaries/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| GIS WebTech (ArcGIS Online) (services6.arcgis.com) | 377 | 1,576 | US | json | [1125 Weems St Parcel\_62Property Outline…](https://services6.arcgis.com/BAJNi3EgCdtQ1BCG/ArcGIS/rest/services/1125%20Weems%20St%20Parcel_62Property%20Outline%20Publish-62%20271/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| HNTB GeoShare (ArcGIS Online) (services.arcgis.com) | 270 | 2,457 | US | json | [2020\_Census\_Texas\_Smooth\_MPO\_UA\_Boundar…](https://services.arcgis.com/rD2ylXRs80UroD90/ArcGIS/rest/services/2020_Census_Texas_Smooth_MPO_UA_Boundaries/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| County of Los Angeles (ArcGIS Online) (services.arcgis.com) | 262 | 1,896 | US | json | [2020\_Census\_Designated\_Places\_WFL1](https://services.arcgis.com/RmCCgQtiZLDCtblq/ArcGIS/rest/services/2020_Census_Designated_Places_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| HDR ArcGIS Online (ArcGIS Online) (services.arcgis.com) | 233 | 2,137 | US | json | [AGOL\_I10Parcels\_CA](https://services.arcgis.com/04HiymDgLlsbhaV4/ArcGIS/rest/services/AGOL_I10Parcels_CA/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| ArcGIS Online for Maryland (ArcGIS Online) (services.arcgis.com) | 226 | 2,537 | US | json | [2022\_General\_Election\_Voting\_Sites\_WFL1](https://services.arcgis.com/njFNhDsUCentVYJW/ArcGIS/rest/services/2022_General_Election_Voting_Sites_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |

</details>

### 🧪 Evals and testing: Varied responses to test tool calls and parsers

**751,070** endpoints · 23,179 services · country US · 2 formats · Run your tool calls against a fixed set of URLs across formats and record which answer; last_tested is the baseline for your own re-tests.

Start with: the whole pack

Example: [Áreas\_Eco\_Oro](https://services.arcgis.com/F7DSX1DSNSiWmOqh/ArcGIS/rest/services/%C3%81reas_Eco_Oro/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) · The Nature Conservancy (ArcGIS Online) · passed 2026-11-16

<details>
<summary>Recommended starting points: 8 services, picked by the stated criteria inside</summary>

**Recommended starting points.** Selected by stated criteria, not a ranking of quality: Services in this pack that returned the most different formats, then the most endpoints that passed a data call, then by name: a mix of response shapes to test parsers and tool calls. Here the services returned 1 format each, so the order comes down to endpoint counts. Only services with at least one bucket row that matches the focus rule are listed, and the sample comes from those rows; the counts cover the whole bucket. The sample URL is the first row by URL sort after preferring, in this order: rows that match the bucket's sample preference when it has one, rows that return values rather than describe a dataset or a service (not ERDDAP /info/ pages, OGC GetCapabilities requests, bare OWS addresses, PxWeb tables, UN SDG series lists, Statistics Canada download pointers, WorldPop listings, GTFS validation reports, untitled rows or service root addresses), and agent-ready rows. Services named "ArcGIS organization" hold map layers from many owners and are added only when fewer than 5 other services match.

| Service (host) | Endpoints in bucket | In pack | Country codes in bucket | Formats in bucket | Sample URL that passed |
|---|---:|---:|---|---|---|
| The Nature Conservancy (ArcGIS Online) (services.arcgis.com) | 3,303 | 3,303 | US | json | [Áreas\_Eco\_Oro](https://services.arcgis.com/F7DSX1DSNSiWmOqh/ArcGIS/rest/services/%C3%81reas_Eco_Oro/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| NOAA GeoPlatform (ArcGIS Online) (services2.arcgis.com) | 3,045 | 3,045 | US | json | [0Z\_850mbHeightsWinds](https://services2.arcgis.com/C8EMgrsFcRFL6LrL/ArcGIS/rest/services/0Z_850mbHeightsWinds/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Africa GeoPortal (ArcGIS Online) (services8.arcgis.com) | 2,938 | 2,938 | US | json | [électrique\_saly](https://services8.arcgis.com/oTalEaSXAuyNT7xf/ArcGIS/rest/services/%C3%A9lectrique_saly/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| FEMA AGOL (ArcGIS Online) (services.arcgis.com) | 2,706 | 2,706 | US | json | [02\_Structures\_Display](https://services.arcgis.com/XG15cJAlne2vxtgt/ArcGIS/rest/services/02_Structures_Display/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Georgia Association of Regional Commissions (ArcGIS Online) (services1.arcgis.com) | 2,703 | 2,703 | US | json | [2010\_Census\_Tracts\_with\_Disadvantaged\_C…](https://services1.arcgis.com/Ug5xGQbHsD8zuZzM/ArcGIS/rest/services/2010_Census_Tracts_with_Disadvantaged_Communities_Data/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| ArcGIS Online for Maryland (ArcGIS Online) (services.arcgis.com) | 2,537 | 2,537 | US | json | [12DigitPivotYearsData](https://services.arcgis.com/njFNhDsUCentVYJW/ArcGIS/rest/services/12DigitPivotYearsData/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| HNTB GeoShare (ArcGIS Online) (services.arcgis.com) | 2,457 | 2,457 | US | json | [1000\_FT\_Buffer\_SR70\_66](https://services.arcgis.com/rD2ylXRs80UroD90/ArcGIS/rest/services/1000_FT_Buffer_SR70_66/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| National Audubon Society (ArcGIS Online) (services1.arcgis.com) | 2,223 | 2,223 | US | json | [Áreas\_clave\_para\_la\_Biodiversidad\_KBA\_c…](https://services1.arcgis.com/lDFzr3JyGEn5Eymu/ArcGIS/rest/services/%C3%81reas_clave_para_la_Biodiversidad_KBA_con_estado_IBA_confirmado_Peru/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |

</details>

The same lists are in [recommended.json](recommended.json), ready for an agent to load.

## Questions an agent can answer with this pack

- Which conservation and habitat layers does The Nature Conservancy publish? Try [Áreas\_Eco\_Oro](https://services.arcgis.com/F7DSX1DSNSiWmOqh/ArcGIS/rest/services/%C3%81reas_Eco_Oro/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (The Nature Conservancy (ArcGIS Online), passed 2026-11-16).
- Which Maryland layers can an agent query on ArcGIS Online for Maryland? Try [12DigitPivotYearsData](https://services.arcgis.com/njFNhDsUCentVYJW/ArcGIS/rest/services/12DigitPivotYearsData/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (ArcGIS Online for Maryland (ArcGIS Online), passed 2026-11-16).
- Which regional layers do the Georgia regional commissions publish? Try [2010\_Census\_Tracts\_with\_Disadvantaged\_Communities…](https://services1.arcgis.com/Ug5xGQbHsD8zuZzM/ArcGIS/rest/services/2010_Census_Tracts_with_Disadvantaged_Communities_Data/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (Georgia Association of Regional Commissions (ArcGIS Online), passed 2026-11-16).
- Which bird and habitat layers does the National Audubon Society publish? Try [Áreas\_clave\_para\_la\_Biodiversidad\_KBA\_con\_estado\_…](https://services1.arcgis.com/lDFzr3JyGEn5Eymu/ArcGIS/rest/services/%C3%81reas_clave_para_la_Biodiversidad_KBA_con_estado_IBA_confirmado_Peru/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (National Audubon Society (ArcGIS Online), passed 2026-11-16).

## What "passed a data call" means

> [!NOTE]
> On the date in `last_tested` (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The `format` column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 16–17 Nov 2026; snapshot 16 Nov 2026.

## For AI agents

Start from keyless JSON endpoints (`agent-ready`). The code below loads `recommended.json` and calls the first recommended service in the Agent tools bucket, with a timeout (`node examples/agent-start.mjs --recommended`). With no argument, `node examples/agent-start.mjs` calls the most recently tested agent-ready row of the sample; pass a `.csv` or `.csv.gz` path to use that file instead. See [examples/agent-start.mjs](examples/agent-start.mjs).

```js
// Node 18+. Loads recommended.json (the local copy, or the raw file on GitHub) and calls one keyless JSON endpoint.
import fs from 'node:fs';

const RAW = 'https://raw.githubusercontent.com/agentpopulation/750k-united-states-apis-for-agents/main/recommended.json';
const rec = fs.existsSync('recommended.json')
  ? JSON.parse(fs.readFileSync('recommended.json', 'utf8'))
  : await (await fetch(RAW)).json();

const pick = rec.buckets.find((b) => b.id === 'agent').services[0];
try {
  const res = await fetch(pick.sample_url, {
    headers: { 'User-Agent': 'agent-example/1.0' },
    signal: AbortSignal.timeout(15000),
  });
  console.log(pick.service, res.status, res.headers.get('content-type'));
  console.log((await res.text()).slice(0, 300));
} catch (err) {
  console.log(`did not answer now; last passed ${pick.sample_last_tested} (${err.message})`);
}
```

How an agent picks an endpoint:

1. Filter to `agent-ready` and your country or topic.
2. Prefer the newest `last_tested` and the larger services.
3. Call with a timeout and check the body before you use it.

## Quick start

The examples run against the sample in `data/` out of the box (1,000 rows). Each takes an optional path to a `.csv` or `.csv.gz` file instead.

```bash
git clone https://github.com/agentpopulation/750k-united-states-apis-for-agents.git
cd 750k-united-states-apis-for-agents
python examples/quickstart.py
node examples/quickstart.mjs
node examples/agent-start.mjs
```

Full list: download `United_States_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz` (751,070 rows, 14.9 MB) from [releases/latest](https://github.com/agentpopulation/750k-united-states-apis-for-agents/releases/latest), then gunzip it and pass its path. The scripts also read the `.csv.gz` as it is.

```bash
gunzip United_States_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz
python examples/quickstart.py United_States_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv
node examples/quickstart.mjs United_States_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv
```

### curl

Quote the URL: some contain commas.

```bash
curl -sL "https://raw.githubusercontent.com/agentpopulation/750k-united-states-apis-for-agents/main/data/United_States_API_Endpoints_AgentPopulation_Sample.csv" | head -n 4
curl -s --max-time 15 "https://services.arcgis.com/F7DSX1DSNSiWmOqh/ArcGIS/rest/services/%C3%81reas_Eco_Oro/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json" | head -c 600
```

### Python

Standard library only: [examples/quickstart.py](examples/quickstart.py) reads the sample, or the path you pass, keeps agent-ready rows and calls the most recently tested one.

<details>
<summary>The code</summary>

```python
# Python 3, standard library only. Run from a clone of this repository:
#   python examples/quickstart.py [path]
# With no path it reads the sample in data/. Pass the full list from the latest release (.csv or .csv.gz) instead.
# Keeps agent-ready rows and calls the most recently tested one.
import csv
import gzip
import os
import re
import sys
import urllib.request

HERE = os.path.dirname(os.path.abspath(__file__))
path = sys.argv[1] if len(sys.argv) > 1 else os.path.join(HERE, "..", "data", "United_States_API_Endpoints_AgentPopulation_Sample.csv")
opener = gzip.open if path.endswith(".gz") else open
with opener(path, "rt", newline="", encoding="utf-8") as f:
    rows = list(csv.DictReader(f))

agent = [r for r in rows if "agent-ready" in r["tags"].split("|")]
# Newest test date first; URLs that describe a dataset or a service rather than return values go last.
DESCRIBES = re.compile(r"/erddap/info/|action-report\.json$|[?&]request=getcapabilities|/GeoArea/[^/?]+/List|getFullTableDownloadCSV|hub\.worldpop\.org", re.I)
agent.sort(key=lambda r: r["last_tested"], reverse=True)
agent.sort(key=lambda r: 1 if DESCRIBES.search(r["url"]) else 0)
print(len(rows), "rows,", len(agent), "agent-ready")
if not agent:
    sys.exit(0)

row = agent[0]
req = urllib.request.Request(row["url"], headers={"User-Agent": "agent-example/1.0"})
try:
    with urllib.request.urlopen(req, timeout=15) as res:
        body = res.read(1_000_000).decode("utf-8", "replace")
        print(res.status, res.headers.get("Content-Type"))
        print(body[:300])
except Exception as err:
    print(f"did not answer now; last passed {row['last_tested']} ({err})")
```

</details>

### JavaScript

Reads the sample as JSON because the CSV has quoted commas.

<details>
<summary>The code</summary>

```js
// Node 18+. Reads the sample as JSON (the CSV has quoted commas), local file first.
import fs from 'node:fs';

const FILE = 'data/United_States_API_Endpoints_AgentPopulation_Sample.json';
const rows = fs.existsSync(FILE)
  ? JSON.parse(fs.readFileSync(FILE, 'utf8'))
  : await (await fetch('https://raw.githubusercontent.com/agentpopulation/750k-united-states-apis-for-agents/main/data/United_States_API_Endpoints_AgentPopulation_Sample.json')).json();

const row = rows.find((r) => r.tags.includes('agent-ready'));
const res = await fetch(row.url, { headers: { 'User-Agent': 'agent-example/1.0' }, signal: AbortSignal.timeout(15000) });
console.log(res.status, (await res.text()).slice(0, 300));
```

</details>

### Agent tools

[examples/agent-tools.json](examples/agent-tools.json) holds two tool definitions in the shape most tool-calling APIs accept (name, description, JSON Schema); rename `parameters` if yours uses another key. [examples/quickstart.mjs](examples/quickstart.mjs) implements them:

- `find_endpoints` searches the agent-ready rows of the list by words (their format is json). When you load the tools of more than one pack, prefix the names (for example `united_states_find_endpoints`) so they do not clash.
- `fetch_endpoint` calls one URL, **refuses any URL that is not in the list** and does not follow redirects. The allowlist is built from the CSV, so a URL injected into a prompt is refused.

The same two tools can sit behind an MCP server.

## Test it yourself

Re-test endpoints from the sample with the same rule: HTTP 2xx and a non-empty body that is not an HTML page. Node 18+, no packages.

```bash
node tools/test-endpoints.mjs
```

It tests the first 50 URLs and prints one line: tested, passed, did not pass. Options: a `.csv` or `.csv.gz` path (the full list from the release), `--limit 50`, `--timeout-ms 10000`, `--out results.csv`. The results file holds `url`, `status`, `passed`, `content_type`, `ms` and `checked_at`; a status of `timeout` or `error:<code>` means no HTTP answer came back. It is polite: GET only, no key sent, at most 4 requests in flight, one at a time per listed host, at least 1 second between requests to one listed host, and reading stops once 256 kB of a body is kept. Redirects are followed and may lead to another host. `results.csv` is in `.gitignore`.

## Preview

One row from each of the five largest services among rows that match the focus rule, services with rows that return values first.

| Title | Service | Country | Format | Tested | Link |
|---|---|---|---|---|---|
| Áreas\_Eco\_Oro | The Nature Conservancy (ArcGIS Online) | US | json | 2026-11-16 | [services.arcgis.com](https://services.arcgis.com/F7DSX1DSNSiWmOqh/ArcGIS/rest/services/%C3%81reas_Eco_Oro/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) |
| électrique\_saly | Africa GeoPortal (ArcGIS Online) | US | json | 2026-11-16 | [services8.arcgis.com](https://services8.arcgis.com/oTalEaSXAuyNT7xf/ArcGIS/rest/services/%C3%A9lectrique_saly/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) |
| 2010\_Census\_Tracts\_with\_Disadvantaged\_Communities\_Data | Georgia Association of Regional Commissions (ArcGIS Online) | US | json | 2026-11-16 | [services1.arcgis.com](https://services1.arcgis.com/Ug5xGQbHsD8zuZzM/ArcGIS/rest/services/2010_Census_Tracts_with_Disadvantaged_Communities_Data/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) |
| 0Z\_850mbHeightsWinds | NOAA GeoPlatform (ArcGIS Online) | US | json | 2026-11-16 | [services2.arcgis.com](https://services2.arcgis.com/C8EMgrsFcRFL6LrL/ArcGIS/rest/services/0Z_850mbHeightsWinds/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) |
| 12DigitPivotYearsData | ArcGIS Online for Maryland (ArcGIS Online) | US | json | 2026-11-16 | [services.arcgis.com](https://services.arcgis.com/njFNhDsUCentVYJW/ArcGIS/rest/services/12DigitPivotYearsData/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) |

Browse the 1,000-row sample: [Sample CSV](data/United_States_API_Endpoints_AgentPopulation_Sample.csv) · [Sample JSON](data/United_States_API_Endpoints_AgentPopulation_Sample.json).

## What's inside

<p align="center"><img src="assets/breakdown.svg" width="100%" alt="Top categories and formats in this pack"></p>

<details>
<summary>Categories: top 8</summary>

| Category | Endpoints | |
|---|---:|---|
| Navigation & Geo/Maps | 310,789 | `████████████████████` |
| Government & Open Data | 245,073 | `███████████████▊` |
| Transport & Mobility | 56,096 | `███▋` |
| Environment | 30,809 | `██` |
| Hydrology & Oceans | 28,895 | `█▉` |
| Health | 18,441 | `█▏` |
| Statistics & Economy | 15,173 | `█` |
| Hazards | 13,262 | `▉` |

</details>

Formats: json 751,069 · geojson 1

<details>
<summary>Largest services: top 25 of 23,179</summary>

| Service | Host | Endpoints | Keyless JSON | |
|---|---|---:|---:|---|
| ArcGIS Online layers (services7.arcgis.com, org 2yAm9dFr5Sk8XULx) † | services7.arcgis.com | 9,876 | 9,876 | `████████████████████` |
| ArcGIS Online layers (services5.arcgis.com, org P4xL2mHKYJn1aLHf) † | services5.arcgis.com | 3,755 | 3,755 | `███████▋` |
| The Nature Conservancy (ArcGIS Online) | services.arcgis.com | 3,303 | 3,303 | `██████▊` |
| ArcGIS Online layers (services1.arcgis.com, org Laaqu2LACymfAn5i) † | services1.arcgis.com | 3,229 | 3,229 | `██████▌` |
| NOAA GeoPlatform (ArcGIS Online) | services2.arcgis.com | 3,045 | 3,045 | `██████▏` |
| Africa GeoPortal (ArcGIS Online) | services8.arcgis.com | 2,938 | 2,938 | `██████` |
| FEMA AGOL (ArcGIS Online) | services.arcgis.com | 2,706 | 2,706 | `█████▌` |
| Georgia Association of Regional Commissions (ArcGIS Online) | services1.arcgis.com | 2,703 | 2,703 | `█████▌` |
| ArcGIS Online for Maryland (ArcGIS Online) | services.arcgis.com | 2,537 | 2,537 | `█████▏` |
| ArcGIS Online layers (services2.arcgis.com, org I9cUOJUZvdGAJncI) † | services2.arcgis.com | 2,522 | 2,522 | `█████▏` |
| HNTB GeoShare (ArcGIS Online) | services.arcgis.com | 2,457 | 2,457 | `█████` |
| ArcGIS Online layers (services5.arcgis.com, org JWrCRn2sKoxC0XsM) † | services5.arcgis.com | 2,346 | 2,346 | `████▊` |
| National Audubon Society (ArcGIS Online) | services1.arcgis.com | 2,223 | 2,223 | `████▌` |
| HDR ArcGIS Online (ArcGIS Online) | services.arcgis.com | 2,137 | 2,137 | `████▍` |
| U.S. Forest Service (ArcGIS Online) | services1.arcgis.com | 2,115 | 2,115 | `████▎` |
| Oregon ArcGIS Online (ArcGIS Online) | services.arcgis.com | 2,089 | 2,089 | `████▎` |
| City of Washington, DC (ArcGIS Online) | services.arcgis.com | 2,047 | 2,047 | `████▏` |
| County of Los Angeles (ArcGIS Online) | services.arcgis.com | 1,896 | 1,896 | `███▉` |
| ArcGIS Online layers (services2.arcgis.com, org U37S3OTVbnXXjTBq) † | services2.arcgis.com | 1,749 | 1,749 | `███▌` |
| Wild Bird Trust (ArcGIS Online) | services7.arcgis.com | 1,707 | 1,707 | `███▌` |
| ArcGIS Online layers (services.arcgis.com, org jDGuO8tYggdCCnUJ) † | services.arcgis.com | 1,694 | 1,694 | `███▍` |
| ArcGIS Online layers (services8.arcgis.com, org 9pNClJ36UGcgthXy) † | services8.arcgis.com | 1,616 | 1,616 | `███▎` |
| ArcGIS Online layers (services.arcgis.com, org ycIuRaoIC4UuCDAS) † | services.arcgis.com | 1,592 | 1,592 | `███▎` |
| GIS WebTech (ArcGIS Online) | services6.arcgis.com | 1,576 | 1,576 | `███▎` |
| Hawaiʻi Statewide GIS Program (ArcGIS Online) | services.arcgis.com | 1,498 | 1,498 | `███` |

† No row of these services matches the focus rule: the selection rule put them in this pack, so they are not used as a starting point.

</details>

<details>
<summary>Rows per test date: 16–17 Nov 2026</summary>

| Date (IST) | Endpoints | |
|---|---:|---|
| 2026-11-17 | 2,106 | `▏` |
| 2026-11-16 | 748,964 | `████████████████████` |

</details>

## Files

| File | Rows | Size | Use |
|---|---:|---:|---|
| [data/United_States_API_Services_AgentPopulation.csv](data/United_States_API_Services_AgentPopulation.csv) | 23,179 | 1.5 MB | One row per service with its endpoint count in this pack |
| [data/United_States_API_Endpoints_AgentPopulation_Sample.csv](data/United_States_API_Endpoints_AgentPopulation_Sample.csv) | 1,000 | 295.2 kB | The sample: focus-rule rows first, each service in proportion to its share; ArcGIS Online layers count as one service |
| [data/United_States_API_Endpoints_AgentPopulation_Sample.json](data/United_States_API_Endpoints_AgentPopulation_Sample.json) | 1,000 | 478.1 kB | The same rows as JSON, tags as an array |
| [United_States_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz](https://github.com/agentpopulation/750k-united-states-apis-for-agents/releases/latest) | 751,070 | 14.9 MB | The full list, gzipped CSV: a download from the latest release, checked by `SHA256SUMS.txt` |
| [tools/test-endpoints.mjs](tools/test-endpoints.mjs) | | | Re-tests endpoints from the sample or the full list |

Sample size: 1,000 rows, which is 1,000 or one third of the pack rounded down, whichever is smaller. Rows that match the focus rule come first. Each service gets rows in proportion to its share of those rows, at least one for the largest services and at most 50% of the sample while other services have rows; ArcGIS Online layers count as one service, whatever their organisation. Within a service, agent-ready rows, rows that return values and the newest test dates come first, and rows are written in turn across services. Service root addresses are placed at the end of the sample.

Full list: download `United_States_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz` (751,070 rows, 14.9 MB) from [releases/latest](https://github.com/agentpopulation/750k-united-states-apis-for-agents/releases/latest), then gunzip it and pass its path. The scripts also read the `.csv.gz` as it is.

Excel users: Data > From Text/CSV, UTF-8. Files are UTF-8 without a byte-order mark and comma-separated.

## Columns and tags

<details>
<summary>Columns, types and tags</summary>

| Column | Type | Example | Meaning |
|---|---|---|---|
| url | string | [https://services.arcgis.com/F7DSX1DSNSi…](https://services.arcgis.com/F7DSX1DSNSiWmOqh/ArcGIS/rest/services/%C3%81reas_Eco_Oro/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) | The address that was tested |
| title | string | Áreas\_Eco\_Oro | Station, dataset or feed name |
| service | string | The Nature Conservancy (ArcGIS Online) | The service the endpoint belongs to; joins to the services file together with host |
| host | string | services.arcgis.com | Host name of the address |
| country | string | US | ISO 3166-1 alpha-2 code, or EU; empty when global or unknown |
| category | string | Navigation & Geo/Maps | Category of the endpoint |
| subcategory | string |  | Left empty from the 15 Nov 2026 snapshot; kept so the columns stay the same |
| format | string | json | What the test call returned: json, csv, geojson, xml, gtfs, zip, txt and so on |
| tags | string | `no-key\|json\|agent-ready` | Tags separated by \| |
| last_tested | date | 2026-11-16 | Date of the test call, YYYY-MM-DD (IST) |

| Tag | Rows | Meaning |
|---|---:|---|
| no-key | 751,070 | No key was sent in the test call |
| agent-ready | 751,069 | No key sent, JSON body, passed a data call on last_tested |
| json | 751,069 | Format of the body |
| geojson | 1 | Format of the body |

A machine-readable copy of this dictionary is in [datapackage.json](datapackage.json).

</details>

## Known limits

- 751,070 rows are map-layer queries with resultRecordCount set: the tested call asked for a few records; change the query to get the full layer.
- 739,487 rows are layers on ArcGIS Online, where anyone can publish: some are class projects, tests or copies. Check the owner and the fields before you rely on one. Only layers of organisations with a name of their own, whose titles do not read as a test, draft or copy, are used as starting points.
- 36,625 rows have a title that reads as a test, a draft, a copy or a sample; they are not used as starting points.
- The country code (US) is the code the endpoint is filed under, not the place the data covers and not always the publisher's country. Where a row had no code, the code of its ArcGIS organisation is used when that organisation lists one country only. In a sample of 40 titles read before release, about 6 were about a place outside the United States. Filter by title or service if you need data about one place.
- Stations and feeds can go quiet after their test date; re-test a URL before you rely on it.
- Not in this pack: endpoints that need a key or a POST, and URLs that did not pass.
- Left out: 1,036 rows with an email-like address.
- Left out: 13,687 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 358 class-exercise copies of the same few ArcGIS Online layers (Miami Beach sea level rise, high-risk areas without shelter, flooded areas, sea level rise and storm surge maps) across many organisations, many with a person's name in the title.
- Left out: 802 layers marked editable in the title (they can hold entries that people added).
- Left out: 97 police traffic-stop layers (they can hold details of people stopped).
- Left out: 2,034 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 3 rows whose address or title held a token-like string, a private address or a similar string.
- Left out: 97,699 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 7,760 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Left out: 5,405 ArcGIS layers that are records about named people (employee, patient, client or donor lists, home addresses, voter lists, sex offender and missing person layers).
- Left out: 839 rows that are another address of an ArcGIS layer dropped for what it holds (one of the reasons above, found under another address of the layer).
- Left out: 9,901 rows of ArcGIS Online organisations that are class accounts (25 layers or more, at least 50% of them class or coursework layers): their other layers are students' work too.
- Left out: 153,426 rows of ArcGIS Online organisations that are class accounts (3 class sets or more in at least 20% of their rows, 10 class sets or more with no organisation name, or layers signed by students read by hand): their other layers are students' work too.
- Left out: 35,772 rows of class sets: one map layer saved under 5 or more students' initials or names in one ArcGIS Online organisation, or in 4 or more students' own organisations.
- Left out: 377,724 rows of university, college and school organisations and hosts (many of their layers are students' work).
- Left out: 1,613 rows whose address is already in an earlier pack of the collection.
- Left out: 240,152 rows that are another address form of an ArcGIS layer already in an earlier pack of the collection (the same rows under another query).
- Left out: 293,504 rows that are a second address form of an ArcGIS layer in this list (the same rows under another query); one address is kept per layer, the newest test first.

## Licence and credit

> [!IMPORTANT]
> This list (URLs, titles, tags and test results) is © 2026 AgentPopulation, released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Credit AgentPopulation and link agentpopulation.com. The data each endpoint returns belongs to its provider and stays under that provider's terms; this licence does not cover it.

Copy-ready credit:

`United States API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 16 Nov 2026.`

GitHub's "Cite this repository" button reads [CITATION.cff](CITATION.cff).

<!-- agentpopulation:start -->
## Part of 10M API endpoints for AI agents

This pack is one of the 50 topic packs of [10m-open-apis-for-ai-agents](https://github.com/agentpopulation/10m-open-apis-for-ai-agents), the open collection by [AgentPopulation](https://agentpopulation.com). Target: 10 million+ open API endpoints that pass a keyless API call.

AgentPopulation's test run of 16 Nov 2026: 4,452,803 tested, 3,346,053 passed a data call. This is the United States pack: 751,070 endpoints from 23,179 services, none of them in a pack read from the earlier snapshot, by address or as another address of the same map layer. Packs overlap, so an endpoint can appear in more than one.

For the latest tested endpoints, search [agentpopulation.com/apis](https://agentpopulation.com/apis). This pack is a snapshot from 16 Nov 2026.

Sibling packs that share the most URLs with this one: [160k-county-and-city-gis-apis-for-agents](https://github.com/agentpopulation/160k-county-and-city-gis-apis-for-agents) (138,206 shared) · [47k-public-agency-gis-apis-for-agents](https://github.com/agentpopulation/47k-public-agency-gis-apis-for-agents) (40,279 shared) · [25k-arcgis-server-apis-for-agents](https://github.com/agentpopulation/25k-arcgis-server-apis-for-agents) (11,583 shared) · [59k-europe-region-arcgis-apis-for-agents](https://github.com/agentpopulation/59k-europe-region-arcgis-apis-for-agents) (5,907 shared). The rest are listed in [10m-open-apis-for-ai-agents](https://github.com/agentpopulation/10m-open-apis-for-ai-agents).

Questions, pack requests, reports of endpoints that stopped answering and requests to remove a row go to [Discussions](https://github.com/agentpopulation/10m-open-apis-for-ai-agents/discussions), or to [@agentpopulation](https://x.com/agentpopulation) on X. The packs are a work in progress and corrections are welcome.

Spotted a wrong row or a dead URL? Tell us on X: [@agentpopulation](https://x.com/agentpopulation).

If this pack saved you time, a star helps others find it.

---

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · [10m-open-apis-for-ai-agents](https://github.com/agentpopulation/10m-open-apis-for-ai-agents)

<!-- agentpopulation:end -->
