# Screenshot evidence — original project workflow

Six user-supplied screenshots were selected because each captures a distinct phase of the real NYC/LA restaurant contact enrichment workflow. Images were copied without altering displayed data. Two tiny cropped title-bar images, overlapping raw snapshots and one screenshot with a Snipping Tool pop-up were excluded.

| Filename | Phase | What the screenshot directly shows |
|---|---|---|
| [`01_nyc_original_csv.png`](../screenshots/01_nyc_original_csv.png) | Original source | NYC inspection source in Excel; CAMIS, establishment, address components and phone fields. |
| [`02_la_original_csv.png`](../screenshots/02_la_original_csv.png) | Original source | Los Angeles OSM source in Excel; object IDs, URLs, coordinates, restaurant names and cuisine. |
| [`03_nyc_power_query_cleaning.png`](../screenshots/03_nyc_power_query_cleaning.png) | Power Query cleaning | NYC Power Query Editor, selected columns and visible applied transformation steps (intermediate state). |
| [`04_la_power_query_cleaning.png`](../screenshots/04_la_power_query_cleaning.png) | Power Query cleaning | Los Angeles Power Query Editor, cleaned records and applied transformation steps (intermediate state). |
| [`05_nyc_final_directory.png`](../screenshots/05_nyc_final_directory.png) | Enriched delivery | Excel NYC five-field final directory with business names, addresses and enriched contact fields. |
| [`06_la_final_directory.png`](../screenshots/06_la_final_directory.png) | Enriched delivery | Excel LA five-field final directory with business names, addresses and enriched contact fields. |

## Interpretation and limitations

- The NYC and LA Power Query screenshots capture intermediate states with **424** and **84** rows visible in the editor respectively, not the final released **414** and **74** records.
- Final worksheet screenshots show a sample of the prepared directories, not every row or evidence of individual contact ownership.
- The screenshots demonstrate Excel and Power Query usage. They are not substitutes for the exported data, QA checks or a comprehensive source-verification log.
- No synthetic or reconstructed interface screenshots were added.
