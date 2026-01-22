# OSINT Case Study 04 (UK) — KYC / EDD Lite on a UK Limited Company (Public Records Only)

**Status:** Public, reproducible (Companies House + Gazette)  
**Data sensitivity:** No private data. Personal addresses/DOB not reproduced in this report.  
**Purpose:** Demonstrate an entry-level EDD-lite workflow using open UK corporate records.  
**Important limitation:** This is not a substitute for regulated KYC/AML checks and does not use paid databases.

---

## Scenario (Public / Training)
A basic EDD-lite check is required on a UK private limited company to support a low-risk onboarding decision.

---

## Objectives
1. Confirm the legal entity exists and capture core identifiers.
2. Identify controllers (PSC) and key officers (at a high level).
3. Review filing history for status changes or notable administrative signals.
4. Check for strike-off signals via The Gazette.
5. Produce a clear, evidence-led risk summary.

---

## Scope and Safety
- **Open sources only** (Companies House, The Gazette, limited open web checks).
- No paid databases (no World-Check / Dow Jones / LexisNexis).
- No collection of sensitive personal information (no DOB, no residential addresses copied).
- This report avoids speculation and sticks to what can be evidenced.

---

## Target Entity (as per Companies House)
**Company name:** GORE CONSULTANCY LIMITED  
**Company number:** 10574295  
**Jurisdiction:** UK (Companies House register)  
**Company type:** Private limited company  
**Incorporated:** 20 January 2017  
**Status shown:** Active — Active proposal to strike off

(See Evidence Log for direct links.)

---

## Method (Step-by-step)

### Step 1 — Entity confirmation (Companies House overview)
Captured:
- Company name and number
- Incorporation date
- Current status and any flags
- Registered office (stored internally; not reproduced in full here)

Output: Entity confirmed as present on Companies House with an “active proposal to strike off” status.

---

### Step 2 — Control & management (PSC + officers)
Reviewed:
- Persons with Significant Control (PSC) register entry
- Officers list (current + resignations)

Output: High-level controller/officer picture captured without copying personal identifiers.

---

### Step 3 — Filing history review (administrative signals)
Reviewed:
- Recent filings (accounts, confirmation statements)
- Address change filings
- Any annotations/rectifications noted by Companies House

Output: A short timeline of notable filings and administrative signals.

---

### Step 4 — Gazette check (strike-off signals)
Checked The Gazette for a “First Gazette Notice” reference matching the company name and number.

Output: The company appears in a First Gazette Notices list (supporting the “active proposal to strike off” status).

---

### Step 5 — Open web presence (minimal)
Light open-web search for the exact company name:
- Basic sanity check for an official website or consistent business presence.
- No deep profiling (this is an entry-level EDD-lite).

Output: Web presence not treated as authoritative; Companies House + Gazette are primary.

---

## Findings (Evidence-led)

### 1) Entity & status
- Companies House lists the company as **Active** with an **“Active proposal to strike off”** flag.
- GOV.UK guidance indicates that strike-off/dissolution processes are publicly recorded and involve Gazette notices.

Interpretation (non-speculative):
- “Active proposal to strike off” is a meaningful operational risk flag. It can indicate either voluntary strike-off or registrar-driven action. Without internal context, the safe stance is: **treat as elevated administrative risk until clarified**.

---

### 2) Control & management (high-level)
- Companies House PSC section shows at least one active PSC entry.
- Officers list shows a mix of current and resigned roles.

Note:
- This report intentionally does not reproduce DOB or full addresses. Those are visible in the original register and should be handled carefully in real screening workflows.

---

### 3) Filing history signals (examples)
Filing history includes:
- Micro-entity accounts filings (multiple years).
- Confirmation statements.
- Registered office address changes over time.
- An annotation on a director appointment filing indicating a partial rectification (address removed from the public register as inaccurate).

Interpretation:
- Micro-entity filings are normal for small companies.
- Address changes can be normal but are also commonly reviewed during onboarding.
- A filing rectification is not automatically “bad,” but it is a compliance note worth recording.

---

### 4) Gazette signal
- The company appears in a **First Gazette Notices** list with the company number.
- This is consistent with Companies House showing an active strike-off proposal.

---

## Risk Summary (EDD-lite)

### Risk rating (portfolio example)
**Overall:** Medium (administrative / continuity risk)  
**Why:** Active proposal to strike off + Gazette notice association.

### Key risk factors (evidence-based)
- “Active proposal to strike off” shown on Companies House.
- First Gazette Notice list reference.

### Practical mitigations / next steps (what I’d do in a real role)
- Ask the counterparty to explain the strike-off status (voluntary closure vs registrar action).
- Request confirmation that the company is trading (recent invoices/contracts, bank letter, or accountant confirmation).
- Confirm whether the company intends to continue operations.
- If onboarding requires it: obtain beneficial ownership confirmation and conduct full AML screening using approved tools (paid databases), plus sanctions/PEP/adverse media checks.

---

## Source Reliability Notes (important)
Companies House explicitly states it performs basic checks but **does not verify the accuracy** of information filed, and the public record should not be treated as validated data. Always corroborate where required.

---

## Evidence Log (reproducible)

| Evidence ID | Source Type | Description | Link |
|---|---|---|---|
| E1 | Companies House | Company overview (status, incorporation) | https://find-and-update.company-information.service.gov.uk/company/10574295 |
| E2 | Companies House | Filing history (accounts, address changes, annotations) | https://find-and-update.company-information.service.gov.uk/company/10574295/filing-history |
| E3 | Companies House | Officers (current/resigned) | https://find-and-update.company-information.service.gov.uk/company/10574295/officers |
| E4 | Companies House | PSC register | https://find-and-update.company-information.service.gov.uk/company/10574295/persons-with-significant-control |
| E5 | Companies House | Service information / disclaimer | https://resources.companieshouse.gov.uk/serviceInformation.shtml |
| E6 | The Gazette | First Gazette Notices list containing company name/number | https://www.thegazette.co.uk/London/issue/829900/supplement/2844/data.pdf |
| E7 | GOV.UK | Strike-off guidance (process overview) | https://www.gov.uk/strike-off-your-company-from-companies-register/apply-to-strike-off |

---

## Reproducible Query Examples
- `site:find-and-update.company-information.service.gov.uk 10574295`
- `"GORE CONSULTANCY LIMITED" 10574295 gazette`
- `site:thegazette.co.uk "GORE CONSULTANCY LIMITED" 10574295`
- `"Active proposal to strike off" Companies House meaning`
