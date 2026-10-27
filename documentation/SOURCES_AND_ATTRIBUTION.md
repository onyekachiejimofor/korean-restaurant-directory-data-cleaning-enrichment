# Public data sources, provenance, and reuse

## New York City
- Original uploaded CSV: `data/raw/nyc_dohmh_restaurant_inspections_download.csv`
- Source: [NYC DOHMH Restaurant Inspection Results (43nn-pn8j)](https://data.cityofnewyork.us/Health/DOHMH-New-York-City-Restaurant-Inspection-Results/43nn-pn8j)
- Uploaded filename indicates extraction dated 2026-10-24; the contained `RECORD DATE` is 2026-10-23.
- 4,538 inspection/citation rows in the supplied extract, with 430 distinct CAMIS identifiers. Not 4,538 distinct establishments.
- The city source includes publicly reported restaurant names, addresses and phone numbers, but not an email/website column.

## Los Angeles area
- Original uploaded CSV: `data/raw/los_angeles_osm_restaurants_download.csv`
- The file contains OSM object identifiers (`osm_type`, `osm_id`, `osm_url`) and OpenStreetMap-derived cuisine, location and contact tags. The exact upstream download service and download time are not available in the uploaded file.
- 2,904 restaurant objects in the supplied extract across many cuisines; 123 cuisine tags contain `korean`.
- **Mandatory OSM attribution:** © OpenStreetMap contributors.
- **OSM data license:** Open Data Commons Open Database License (ODbL); [licensing details](https://www.openstreetmap.org/copyright); [license text](https://opendatacommons.org/licenses/odbl/).
- The ODbL includes attribution and share-alike obligations for covered derived databases. Do not assume a blanket proprietary or MIT license applies to OSM-derived data.

## Manual enrichment
Additional publicly visible business contact data were collected manually by the portfolio author. The final files do not include a complete per-field verification audit trail for each email or website. Do not infer that a populated cell is audited, currently deliverable, or contactable. `quality_assurance/verification_log_TEMPLATE.csv` is supplied for future evidence collection.

## Attribution and usage caution
These files demonstrate data operations methods, not a legal opinion on rights to every individual enrichment source. Retain original provider credits, observe website terms and applicable outreach/privacy law, and respect any additional third-party data reuse restrictions. Do not assert that source publishers or freelance platforms commissioned or endorsed this project.
