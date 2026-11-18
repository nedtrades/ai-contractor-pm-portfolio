# Document Control (ISO 9001-style)

This is how Falcon ICM, LLC numbers, revises, approves and tracks project documents. It follows the document-control ideas in ISO 9001 (control of documented information). It is a working method, not a certification claim.

## 1. Document ID scheme

| Prefix | Type | Example | Notes |
|---|---|---|---|
| QM- | Quality manual and top-level policy | QM-001 | One per company |
| QP- | Procedure | QP-855 Field Service and Turnover | Number tracks the related ISO 9001 clause where it helps (8.5.5 → 855) |
| FM- | Form or template (blank) | FM-855-01 Turnover Checklist | Parent procedure number plus a two-digit form number |
| REG- | Register or log | REG-830 Document Register | Living list; revised by row, not by reissue |
| COM- | Commissioning report (filled) | COM-0000 | One per system or project |
| RFI- / CO- | RFI or change order (filled) | RFI-0000-07 | Project number plus sequence |

The file name always starts with the document ID and revision, for example `FM-855-01_Turnover-Checklist_RevA.md`. The ID in the file name, the header and the register must match. If they do not, the register wins and the file gets corrected.

## 2. Revisions

- Drafts: Rev 0.1, 0.2 and so on. Not for use on a job.
- Approved: Rev A, B, C. A new letter for any change to content.
- Typo-only fixes may keep the letter but must get a change-log row.
- The superseded revision is marked "SUPERSEDED" and moved to the archive folder. It is never deleted.

## 3. Control block (top of every controlled document)

| Field | Value |
|---|---|
| Document ID | |
| Title | |
| Revision | |
| Status | Draft / Approved / Superseded |
| Owner (role) | |
| Prepared by (role) | |
| Reviewed by (role) | |
| Approved by (role) | |
| Approval date | |
| Next review due | |
| AI-assisted? | Yes / No. If yes: drafted with AI, verified by (role) on (date) |

## 4. Approval rules

| Document type | Prepared by | Approved by |
|---|---|---|
| Plumbing procedures, forms and reports | Project Manager or Field Technician | Licensed Plumbing Manager |
| HVAC/R and hydronic procedures, forms and reports | Project Manager or Field Technician | Mechanical Manager |
| Customer-facing letters (turnover, change orders, incident notices) | Project Manager | Licensed Plumbing Manager or Mechanical Manager for the scope |
| Quality manual and procedures | Project Manager | Owner of Falcon ICM, LLC |

Nobody approves their own document. AI-drafted text counts as "prepared by" the person who prompted it; it still needs a separate approver for controlled documents.

## 5. Change log (bottom of every controlled document)

| Rev | Date | Section(s) changed | Description of change | Reason | Prepared by (role) | Approved by (role) |
|---|---|---|---|---|---|---|
| A | 2026-__-__ | All | First approved issue | New document | | |
| | | | | | | |

## 6. Records vs. documents

- A **document** tells you how to do the work (procedure, blank form). It is revised.
- A **record** proves the work was done (filled form, test report, signed turnover). It is never revised. If a record has an error, a new record corrects it and references the original.

## 7. Register

Every controlled document is listed in [`document-register.csv`](document-register.csv): ID, title, revision, status, owner role, approval date and next review date.
