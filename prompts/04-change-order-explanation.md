# 04. Prompt: Change-Order Explanation

```text
Draft a change-order explanation for an approver who is not a plumber or
HVAC technician.

Inputs: CO number, site, what was found (field notes, photo IDs), why it
matters, options with cost and schedule for each (from priced estimates),
our recommendation and reason, decision deadline, what we will do if no
decision arrives by the deadline.

Structure: title; what we found; why it matters to you (in terms of store
operations, downtime, risk of a future repair); options table side by side
(cost, schedule, downtime, risk after turnover); recommendation;
decision needed by; default if no decision.

Rules:
- Show every option given in the inputs, including the lowest-cost one.
- Use only the cost and schedule figures in the inputs. If a figure is
  missing, write [MISSING] and list it under "GAPS FOR REVIEWER".
- Describe risk plainly. Do not give failure probabilities or life
  expectancy unless a cited document provides them.

INPUTS:
[paste here]
```

## Human verification step

Match each cost and schedule figure to the priced estimate on file. Confirm the default action is allowed by the contract. Run the [human verification checklist](00-human-verification-checklist.md). Licensed reviewer for the scope approves.
