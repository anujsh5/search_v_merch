# Search vs Merch Dashboard

Static GitHub Pages dashboard built from the reviewed BigQuery export.

## Publish

Upload all files in this folder to the same GitHub repository directory and enable GitHub Pages. Keep `index.html` and `data.csv` together.

## Files

- `index.html` — dashboard application
- `data.csv` — snapshot covering 2026-07-07 through 2026-07-16

## Metric definitions

- Impressions: sum of impression event counts.
- Clicks: sum of click event counts.
- CTR: filtered clicks divided by filtered impressions.
- Impression-user observations: sum of distinct users at the exported row grain. This is not an overall deduplicated user count across dates, hours, page types, or brands.

## Scope

- Widget tables: widget_id = fr.
- Listing tables: x_id matches prep_<digits>_<alphanumeric>.
- Search: page_type = listing_search.
- Merch: all other page types.
- Time zone: Asia/Kolkata.
