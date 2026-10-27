# Data dictionary

The three CSV deliverables and both city worksheets have exactly these five columns:

| Field | Type / example | Meaning | Missing-value rule |
|---|---|---|---|
| Company Name | Text — `HAEJANG` | Public-facing establishment name | Required; never blank in published snapshot |
| Address | Text — `162-10 Crocheron Avenue, Queens, New York 11358` | Reported physical establishment location | Required; address may still need current external confirmation |
| Email Address | Text — `hello@example.com` | Public business email captured during research | Leave entirely blank if unavailable or unconfirmed |
| Phone Number | Text — `2122233488` or `+1 213-123-4567` | Reported business contact number | Text, not number; preserve prefixes/leading zero possibilities |
| Website | Absolute HTTP(S) URL | Business website/domain; not a restaurant directory listing | Leave blank if no eligible business website established |

The five-field schema intentionally contains no `City`, `Source URL`, `OSM ID`, `CAMIS`, `Verified On`, `Status` or `Reviewer Notes` columns. Those tracking fields belong in supporting source and quality-assurance files so the core client brief remains unchanged.

**Data-quality note:** Full address strings have not been standardized into house-number/street/city/ZIP subcolumns. Syntax checks do not confirm current operation or business ownership.
