# Google Maps Public Business Email Extractor

> An n8n lead-research workflow that turns a list of public business websites into a deduplicated Google Sheets export.

## What it does

The workflow begins with business website URLs gathered from Google Maps, fetches publicly accessible pages, extracts emails that are visibly published on those pages, filters unusable results, splits multiple addresses, and writes the cleaned rows to Google Sheets.

## Workflow map

```text
Google Maps results
  → website URLs
  → public-page fetch
  → email-pattern extraction
  → split / filter / deduplicate
  → Google Sheets export
```

## Output handling

The workflow is intended to create a research list, not a permission to send bulk email. Any later outreach should validate addresses, remove duplicates, check prior contact history, and follow applicable privacy, anti-spam, and platform rules.

## Setup

1. Import `workflow.json` into n8n.
2. Connect the Google Sheet you control.
3. Provide the public business-site URLs from your own permitted source.
4. Set a sensible request rate and timeout.
5. Review extraction output manually before using it for outreach.
6. Add email verification and a suppression list for real operations.

## Responsible use

- Use only business information intentionally made public.
- Respect website terms, rate limits, privacy law, and anti-spam obligations.
- Do not collect sensitive personal data.
- Do not treat a regex match as proof that an inbox is active or suitable for contact.
- Do not use this workflow to evade website protections or access restrictions.

## Repository contents

| File | Purpose |
| --- | --- |
| `workflow.json` | Importable n8n research workflow |
| `SECURITY.md` | Safe-operation guidance |
| `LICENSE` | MIT license |

## License

MIT — see [LICENSE](LICENSE).