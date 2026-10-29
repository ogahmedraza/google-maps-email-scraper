# Google Maps Email Scraper

An n8n lead-research workflow that collects public cleaning-business websites from Google Maps, fetches public pages, extracts publicly listed business emails, removes duplicates, and exports structured results to Google Sheets.

## Flow

`Google Maps search → Website extraction → HTTP requests → JavaScript email extraction → Deduplication → Google Sheets`

## Included

- Website URL processing
- Public HTML fetching
- Public business-email extraction
- Multiple-email splitting
- Empty-result filtering
- Duplicate removal
- Google Sheets export

## Responsible use

Use only publicly available business information, respect website terms and applicable privacy laws, apply rate limits, and avoid collecting sensitive personal data.

## Setup

Import `workflow.json` into n8n and configure your own Google Sheets and HTTP settings. Add validation, rate-limit handling, and email verification before production use.
