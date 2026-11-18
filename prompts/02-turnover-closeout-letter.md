# 02. Prompt: Turnover and Closeout Letter

```text
Draft a turnover letter for a completed plumbing / HVAC/R / hydronic job.
Inputs: site, project number, scope, completed turnover checklist,
commissioning report ID, equipment list, punch list, warranty terms from
the contract, training record.

Structure:
1. One-paragraph opening: what is complete and since when.
2. "What you are receiving": a table of every turnover item and where it
   is (attached document ID, binder location).
3. "Open items": the punch list as a table with owner role and target date.
   Do not leave any open item out.
4. "Warranty": our workmanship terms exactly as given in the inputs, plus
   a line that equipment warranties are the manufacturers'.
5. "First-year recommendations": routine maintenance only, taken from the
   inputs or manufacturer manuals provided. No savings or performance
   claims.
6. Acceptance: how the owner accepts turnover (signed form).

Rules:
- Every item in the turnover checklist that is "Done" must appear in the
  table. Every item that is "Open" must appear in open items.
- Do not add any document, date or term not in the inputs.
- List missing inputs under "GAPS FOR REVIEWER".

INPUTS:
[paste here]
```

## Human verification step

Cross-check the "What you are receiving" table line by line against the actual package. Check warranty language against the contract. Run the [human verification checklist](00-human-verification-checklist.md). Licensed Plumbing Manager or Mechanical Manager signs the letter.
