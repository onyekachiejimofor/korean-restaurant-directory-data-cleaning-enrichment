# Quality assurance report — release snapshot (2026-10-27)

This report applies to the **five-field CSVs and new combined Excel workbook in `data/final/`**, not to the original uploaded source CSVs or the unchanged user workbooks.

## Verified structural checks

| Check | NYC | LA | Total |
|---|---:|---:|---:|
| Data rows | 414 | 74 | 488 |
| Company Name filled | 414 | 74 | 488 |
| Address filled | 414 | 74 | 488 |
| Phone Number filled | 414 | 74 | 488 |
| Email Address filled | 222 | 31 | 253 |
| Website filled after publication review | 306 | 53 | 359 |
| Both email + website filled | 215 | 25 | 240 |
| Exact duplicate normalized name + address keys | 0 | 0 | 0 |
| Email strings failing simple pattern validation | 0 | 0 | 0 |
| Website strings failing simple HTTP(S)-URL format validation | 0 | 0 | 0 |
| Populated phone strings with unexpected digit count (outside 10 or 11) | 0 | 0 | 0 |

## How the numbers were calculated

- `Populated`: nonempty underlying displayed cell values, not Excel internal shared-string indices.
- `Duplicate composite key`: normalized case and repeated whitespace within `(Company Name, Address)`; different branch addresses are distinct records.
- `Email syntax`: simple `local@domain.tld` pattern, not email delivery testing.
- `URL format`: starts with `http://` or `https://` and looks like a domain; neither ownership nor current accessibility was universally verified.
- `Phone structure`: 10 digits, or 11 including country code; not an active-line check.

## Five transparent publication exceptions

The author's last submitted Excel workbooks have been preserved unchanged under `data/submitted_workbooks/`. The GitHub release CSVs and combined deliverable have **five website cells blanked** because the original URLs were plainly directory pages or expressly unofficial. No address, email, phone or business name fields were modified. See `quality_assurance/publication_adjustments.csv` for exact business, original row and URL.

### Before and after publication adjustment
- User's final submitted NYC workbook: 308 populated websites. GitHub release NYC CSV: **306**.
- User's final submitted LA workbook: 56 populated websites. GitHub release LA CSV: **53**.
- User's submitted total: **364** website strings. GitHub release: **359**.

## Outstanding *verification* work (not mechanical spreadsheet errors)

1. Complete the per-field official-source evidence log for populated emails and websites; the manual research trail wasn't provided in a verifiable structured log.
2. Investigate the multi-brand / multi-business records listed in `manual_review_queue.csv`; multiple names in one cell may represent aliases or separate businesses.
3. Recheck operating status of historical or renamed businesses, and whether venues with ambiguous cuisine/activity meet the precise client eligibility definition.
4. Establish a complete source-ID → released-business mapping if a future project promises exhaustive coverage and refreshability.
5. Recheck phone-line activity and branch-specific contact ownership before operational use.

**Release meaning:** structurally clean *portfolio snapshot*. It is not a certified current, exhaustive, real-time verified directory.
