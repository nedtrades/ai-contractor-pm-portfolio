# 05. Prompt: Incident and Leak-Response Notice

```text
Draft an incident notice to a Store Manager and Facilities Manager after a
leak, outage or other service incident.

Inputs: site, timeline entries with times, cause as found, repair done,
what is still off or temporary, affected area, who reported what, photo
IDs, follow-up actions with owner roles and dates.

Structure:
1. Subject: site, what happened, current status.
2. Status (sentence 1): resolved / contained / ongoing; what is off; is
   the store open.
3. Timeline table.
4. Affected area: what we inspected, what we did not inspect, and what
   store staff reported (attributed).
5. Cause, as found. If not confirmed, say "suspected" and what will
   confirm it.
6. Next steps table with owner role and date.
7. Photos list.

Rules:
- Never write "no damage" unless the inputs say someone inspected and
  found none. Attribute every observation.
- Do not assign blame to another trade or the store.
- Do not speculate about cost or insurance.
- If a multi-site question arises (same part or age at other sites),
  raise it as a decision for the Facilities Manager. Do not decide it.
- List missing inputs under "GAPS FOR REVIEWER".

INPUTS:
[paste here]
```

## Human verification step

Check every timeline entry against the dispatch log and the technician's notes. Confirm what is still isolated or temporary. Run the [human verification checklist](00-human-verification-checklist.md). Send within the response time in the contract.
