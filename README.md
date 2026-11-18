# AI-Assisted Project Management and Client Communication for Facility Plumbing and HVAC/R

**Falcon ICM, LLC (Oregon)** · Ned Booher · Oregon Plumbing Business license PB 3483 · Oregon HVAC/R license LHR 784

I use AI tools to write faster, clearer and more complete project documents and client messages. I read, correct and sign every one of them. A licensed professional stays accountable for every word, every reading and every recommendation.

This repo shows how that works on multi-site retail and commercial facility work: the templates I fill, the workflows I run, the prompts I give the AI, and side-by-side examples of a typical contractor note next to the reviewed version a facility manager actually gets.

> **All site names, numbers, dates and readings in this repo are illustrative samples.** Sites are written as "Retail Store #0000, Anytown OR." No client, store, project or person in this repo is real. The before-and-after pairs are illustrative rewrites I wrote to show the method. They are not quotes from real clients or real jobs.

---

## Who this is for

Facility and operations teams that run many stores or buildings and need their plumbing and mechanical contractors to:

- tell them what happened, what it means for the store, and what they need to decide, in the first two lines
- hand over turnover packages that are complete the first time, with readings, serials, warranty dates and as-builts in one place
- explain an RFI or change order so a non-technical approver can say yes or no the same day
- send leak and outage notices that a Store Manager can act on at 6 AM

## Background

- About 25 years in mechanical and plumbing work, centered on hydronic, geothermal (ground-source) and other water-based heating and cooling, on public and private projects.
- Owner of Falcon ICM, LLC, an Oregon specialty contracting business.
- Oregon Plumbing Business license PB 3483 and HVAC/R license LHR 784.

## What AI changes for the customer

| Without AI | With AI plus my review |
|---|---|
| Status notes written from memory at the end of the day, when there is time | A structured update drafted from my field notes and photos the same day, then checked by me |
| Turnover packages assembled at the end of the job, with gaps found by the owner | A turnover checklist that tracks every item from rough-in on, so gaps show up while the crew is still on site |
| Change orders written in trade shorthand | A plain-English explanation of cause, options, cost, schedule and what happens if the owner does nothing |
| One writing style per person on the crew | One house style across every site and every message |

What the AI does **not** do: it does not take readings, make code calls, decide pass or fail, approve work, or sign anything. Those stay with the licensed person on the job.

## How I use AI

1. **Field facts come first.** Readings, photos, serial numbers, test results and times come from the field: from me, my crew, or the instruments. The AI gets those facts as input. It does not supply them.
2. **The AI drafts.** I use the prompts in [`prompts/`](prompts/) to turn notes into a status update, a closeout letter, a change-order explanation or an incident notice, using the templates in [`templates/`](templates/).
3. **Human review gate.** Nothing goes to a customer until I have run the [verification checklist](prompts/00-human-verification-checklist.md): every number checked against the source, every code or spec reference checked against the actual document, every commitment (date, cost, scope) one I can keep. If I cannot verify a sentence, it comes out.
4. **Licensing accountability.** Plumbing and HVAC/R work, and the statements about that work, sit under my Oregon licenses. The AI is a writing tool. The license holder signs, and the license holder answers for it.
5. **No unverified claims.** No made-up performance numbers, savings, or results. No "should be fine." If a reading is pending, the message says pending. If I do not know yet, the message says when I will know.
6. **Customer data stays controlled.** Real site documents follow the customer's rules for where data may go. Anything published, like this repo, is anonymized.

## Before and after (excerpts)

Full pairs, with notes on what changed, are in [`examples/before-after/`](examples/before-after/). These are illustrative rewrites, not real client messages.

**Status update to a Facilities Manager**

> *Before:* Water heater done. Still waiting on the relief valve part. Should be back Thursday maybe.

> *After:* **Retail Store #0000, Anytown OR: water heater replacement, Tuesday update.** The new water heater is installed and running, and the store has hot water. One item is open: the temperature and pressure relief valve that came with the unit was damaged in shipping. A temporary listed valve is installed and the system is safe to operate. The replacement valve is due Thursday, and we will swap it during the store's morning low-traffic window that day. Nothing is needed from you. If the part slips, I will tell you by Wednesday 3 PM.

**Change-order explanation**

> *Before:* CO #3 - found galv line in wall, need to replace 40 ft, add $X.

> *After:* **Change Order #3 (illustrative sample): replace corroded galvanized water line behind the restroom wall.** When we opened the wall for the new fixtures, we found about 40 feet of original galvanized pipe with heavy corrosion at the joints. Reconnecting new fixtures to it risks a leak behind finished walls. Option A: replace the 40 feet now while the wall is open (adds cost and one working day). Option B: connect to the existing pipe and document the condition (no added cost now; higher chance of a future leak and a second wall opening). I recommend Option A. I need a decision by Friday to hold the schedule.

**Leak response notice**

> *Before:* Had a leak at the store last night, fixed it.

> *After:* **Leak at Retail Store #0000: water is off at one fixture, store is open.** At 5:40 AM the Store Manager reported water on the floor in the back-room restroom. Our technician arrived at 6:25 AM, found a failed supply line at the hand sink, shut the fixture's isolation valve and replaced the line. The rest of the building's water was never shut off. Floor area affected: back-room restroom and part of the hallway, cleaned by store staff. No product was damaged according to the Store Manager. Next step: we return Thursday to check the other supply lines in that restroom, which are the same age.

## Repo map

```
.
├── README.md                     This file
├── LICENSE                       MIT, Falcon ICM, LLC
├── examples/
│   └── before-after/             Five illustrative before/after pairs with "what changed" notes
├── templates/                    Blank forms and trackers (Markdown and CSV)
│   ├── turnover-commissioning-checklist.md / .csv   Plumbing, HVAC/R and hydronic turnover items
│   ├── commissioning-report.md                      Functional test and readings report
│   ├── weekly-status-update.md                      One-page weekly update for a facility or store
│   ├── client-correspondence-style-guide.md         House style for every customer message
│   ├── document-control.md                          ISO 9001-style ID, revision, approval and change log
│   ├── document-register.csv                        Master list of controlled documents
│   ├── spec-to-service-record.md                    Design-phase serviceability and baseline record
│   ├── rfi-change-order-log.csv                     RFI and change-order tracker
│   └── punch-list-tracker.csv                       Open items by site, owner role and due date
├── workflows/                    How the work moves (Mermaid diagrams)
│   ├── scheduling-and-handoff.md
│   ├── multi-site-pm-cadence.md
│   └── turnover-handoff.md       Install through commissioning, closeout and warranty
└── prompts/                      Reusable AI prompts, each ending in a human verification step
```

## Roles used in this repo

Every task owner is a role, never a named person: Project Manager, Licensed Plumbing Manager, Mechanical Manager, Facilities Manager, Commissioning Agent, Store Manager, and Field Technician.

## Contact

Ned Booher, Falcon ICM, LLC · ned@falconicm.com

## License

MIT. See [LICENSE](LICENSE). The templates are free to use. A filled form is only as good as the licensed person who checked it.
