# Case brief and business value

## Business request
This project independently replicates a real freelance-style request to gather Korean restaurant contacts in New York City and Los Angeles using five mandatory fields:

1. Company Name
2. Address
3. Email Address
4. Phone Number
5. Website

## Problem statement
Public-source restaurant information is fragmented across inspection datasets, OSM objects, business pages and online directories. A source CSV is not directly suitable for business use: it may contain citation-level duplication, inconsistent address strings, missing website/email fields, and multiple branches under one brand.

## Intended operational use
- Prepare standardized restaurant directory records for CRM or directory onboarding.
- Support responsible, relevant restaurant partnership/vendor research.
- Reduce repeated lookup work when teams research city-specific business contacts.
- Enable human review of missing or uncertain information instead of inventing contact details.

## Deliverable and definition of done
- One row per curated location in each city file.
- Exactly the five requested data fields in delivery tables.
- Legitimate blanks for contacts not found; no synthetic emails.
- No duplicate exact name-and-address composite keys.
- Exceptions and provenance disclosed.
- Source CSV snapshots preserved separately from handoff files.

## Responsible claims
This is a self-directed portfolio replication of a publicly described freelance request. No paid client, employment engagement, Fiverr endorsement, exhaustive coverage or realized financial outcome is claimed. The source extract and final files are snapshots, not a continuously verified directory.
