## United States API endpoints, snapshot 16 Nov 2026

- 751,070 endpoints passed a keyless data call, tested 16–17 Nov 2026 (IST)
- 23,179 services · country US · 751,069 keyless JSON rows

### Download

- `United_States_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz`: the full list, 751,070 rows, 14.9 MB gzipped (246.9 MB as CSV), SHA-256 `fb0cc1010b33f50f16d687c27b79e3471ab7b119e7936b0ddd5f915223156739`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile United_States_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip United_States_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 751,069 · Wrap one layer query as a get_layer_features tool: pass a where clause or a bounding box, return the matching features with a timeout.
- 📱 App features: 751,070 · Add the layers to an app map: read the layer once for its fields, then ask for the features in the visible area.
- 🧠 Grounding and data pipelines: 80,338 · Load the tables and layers on a schedule into your own store, so an agent can cite a dated source.
- 🧪 Evals and testing: 751,070 · Run your tool calls against a fixed set of URLs across formats and record which answer; last_tested is the baseline for your own re-tests.

### Changes

- First release
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
- Overlap: 5,907 of these URLs are also in 59k-europe-region-arcgis-apis-for-agents.
- Overlap: 138,206 of these URLs are also in 160k-county-and-city-gis-apis-for-agents.
- Overlap: 40,279 of these URLs are also in 47k-public-agency-gis-apis-for-agents.
- Overlap: 11,583 of these URLs are also in 25k-arcgis-server-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 16–17 Nov 2026; snapshot 16 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 16 Nov 2026.

Credit: United States API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 16 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
