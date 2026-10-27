# Methodology — How this directory was prepared

## 1. Source assessment
**NYC:** Inspect the DOHMH restaurant-inspection CSV. CAMIS identifies restaurants; multiple violation rows can belong to the same permit holder. Restaurant identity, not inspection-row count, is the relevant unit of the final directory.

**LA:** Inspect the OpenStreetMap-derived restaurant CSV. Check name, cuisine and geographic/address tags; review the Korean-cuisine filter. One OSM object is not automatically a current Korean restaurant.

## 2. Data cleaning with Excel + Power Query
The portfolio creator used Excel and Power Query to clean and reshape the public CSV records before loading them into worksheets. The five required output fields were organized as Company Name, Address, Email Address, Phone Number and Website. Dates/inspection violations/geocoordinates from raw source tables were not included in the five-field client delivery.

Authentic Power Query transformation screenshots are now included in `screenshots/`, showing applied steps from both cities. However, a separately exported, machine-independent `.pq`/M script was not supplied, so this document **does not invent exact M queries or claim a one-click reproducible pipeline**. The original user workbooks retain Power Query-related metadata but refreshing them may depend on paths not available on other computers.

## 3. Manual data entry and web research
The creator manually researched unavailable contact information, including business websites, addresses, phone numbers and emails listed on restaurant-controlled web or social channels. Where no qualifying contact was available, cells were left blank.

A URL that merely mentions a restaurant (directory, review site, third-party listing) is not automatically its official website. A general chain email may not be branch-specific. Several unresolved historical/location cases are recorded in the review queue.

## 4. Composite-key deduplication
Compare normalized Company Name and Address together. Do **not** deduplicate on company name alone: a chain can have multiple branches. Do **not** deduplicate on street address alone: multiple businesses can share a building.

## 5. Quality assurance and publication adjustment
Audit mandatory fields, populated email/website syntax, 10/11-digit phone structure, duplicate composite keys and out-of-scope names. This release excludes five visibly third-party/unofficial website URLs from published CSV/Excel copies, leaving those cells blank. The user's final submitted workbooks are preserved as evidence, unchanged.

## 6. What would make the work fully reproducible
- Screenshots of actual Power Query Applied Steps and source-to-output comparisons.
- An archived query / workbook with portable input paths.
- Per-field source verification links and check dates.
- Explicit review of closed, relocated or cuisine-ambiguous businesses.
- A source ID -> output record identity crosswalk for the whole extract.

These enhancements are honest next steps, not evidence already claimed as done.
