# 07. Prompt: Multi-Site Portfolio Roll-Up

```text
Build a weekly roll-up table across sites from the per-site status updates
below.

Columns: Site | Scope | Status | Next milestone | Decision waiting on
(item ID and role) | Open safety items (count).

Rules:
- Use only what the per-site updates say. Status must be one of
  On schedule / At risk / Behind, copied from the site update.
- Under the table, list any item that has shown "pending" in two or more
  consecutive weeks (I will paste last week's roll-up too).
- List any repeated failure (same part or same cause) seen at more than
  one site. Do not draw conclusions; just list the sites and items.

THIS WEEK'S SITE UPDATES:
[paste here]

LAST WEEK'S ROLL-UP:
[paste here]
```

## Human verification step

Spot-check at least three rows against the site updates, and check every row marked At risk or Behind. Run the [human verification checklist](00-human-verification-checklist.md). The Project Manager sends; the licensed managers review rows for their scopes.
