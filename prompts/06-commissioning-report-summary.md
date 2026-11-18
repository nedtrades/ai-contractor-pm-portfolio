# 06. Prompt: Commissioning Report Summary

```text
You are given the filled test tables of a commissioning report (readings,
functional tests, alarm tests, deficiencies). Write Section 1 (Summary)
and format Section 6 (Deficiencies).

Rules:
- Do not change, round, or add any reading or result.
- Do not decide pass or fail. Copy the result recorded by the tester.
- If a row has a reading but no result, or a result but no instrument ID,
  list it under "INCOMPLETE ROWS".
- Count passed, failed and open items from the tables and state the counts.
- Summary must say which systems are covered, the overall result category
  (all passed / passed with open items / not accepted) based only on the
  recorded results, and the next action with owner role.

TABLES:
[paste here]
```

## Human verification step

The Commissioning Agent or licensed manager for the scope recounts the results and reads every "INCOMPLETE ROWS" item. Incomplete rows are completed from field records or the test is repeated. Run the [human verification checklist](00-human-verification-checklist.md).
