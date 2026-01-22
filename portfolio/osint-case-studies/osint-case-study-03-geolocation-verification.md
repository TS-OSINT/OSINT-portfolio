# OSINT Case Study 03 (UK) — Geolocation Verification Using Public Media (Image + Video)

**Status:** Public, reproducible  
**Data sensitivity:** No personal data. Public sources only.  
**Purpose:** Demonstrate a clear, entry-level geolocation workflow with transparent evidence logging.  
**Notes:** This is a portfolio exercise using Creative Commons media. It is not intended to identify people or facilitate harm.

---

## Scenario (Public / Training)
A short video clip and an aerial photograph were shared without reliable context. The claim was simply that the media shows “a famous London bridge.”

### Objectives
1. Determine the most likely location shown in the media.
2. Confirm the result using at least **two independent anchors** (architecture + map/geodata).
3. Document the steps so another person can reproduce the outcome.

---

## Scope and Safety
- Public sources only (Creative Commons media, Wikipedia/OpenStreetMap-linked references).
- No attempt to identify individuals, vehicles, or private activity.
- No face analysis, no doxxing, no contact.

---

## Inputs (Evidence Items)
**E1 — Aerial photo (image):** “London Tower Bridge 22.jpg” (Wikimedia Commons)  
**E2 — Short clip (video):** “LondonTowerBridge1998Video1.ogv” (Wikimedia Commons)

(Links in the Evidence Log below.)

---

## Method (Step-by-step)

### Step 1 — Capture visual clues (no guessing yet)
From the aerial photo (E1), the following features were noted:
- A large river with multiple piers/bridge approaches.
- A distinctive bridge with two matching stone towers.
- A high-level horizontal walkway between the towers.
- Blue/white suspension-style elements and a roadway deck.
- Surrounding dense urban grid consistent with a major city center.

From the video (E2), additional cues:
- Same twin-tower bridge structure visible at street level.
- The bridge appears to be a bascule (lifting) bridge or has moving parts.
- River traffic and embankment structures consistent with an urban river crossing.

**Working hypothesis:** A landmark bridge in London (candidate list formed in Step 2).

---

### Step 2 — Generate candidate locations (controlled shortlist)
Based on architecture (twin neo-gothic style towers + high-level walkway), likely candidates were:
- Tower Bridge (London)
- (Very low likelihood) other twin-tower bridges with a walkway (rare)

At this stage, the structure strongly suggests **Tower Bridge**, but confirmation is required.

---

### Step 3 — Confirm using independent anchors (architecture + geodata)
**Anchor A (architecture match):**
- Tower Bridge is known for: twin towers, high-level walkways, bascule mechanism, and suspension components.
- Visual match from both E1 and E2 is consistent with these elements.

**Anchor B (geotag / map):**
- The Wikimedia photo page for E1 includes **camera location coordinates** (geotag) at approximately:
  - **51.503288, -0.073905**
- Those coordinates correspond to the Tower Bridge area in London (and the photo is labeled accordingly).

Result: Both anchors converge on **Tower Bridge, London, UK**.

---

## Findings
### Location (Final Assessment)
**Confirmed location:** Tower Bridge, London, United Kingdom  
**Confidence:** High  
**Rationale:** Strong architectural uniqueness + geotagged camera location on the image source page.

---

## Limitations (What this does and does not prove)
- This verifies **location** of the media. It does **not** confirm:
  - who filmed it,
  - the exact date of filming beyond what the uploader states,
  - the intent or original context of the share.
- Wikimedia metadata helps, but in real investigations I would also:
  - preserve original uploads (hashing),
  - check for re-uploads or earlier instances via reverse image/video search,
  - confirm context with additional independent sources.

---

## What I Would Improve Next Time (Practical upgrades)
- Extract keyframes from the video and run reverse image search on 2–3 frames.
- Build a simple “visual anchor list” template (towers, walkway, bascules, suspension details).
- Add a lightweight timeline section if the claim includes a date.

---

## Evidence Log (reproducible)

| Evidence ID | Type | Description | Source | Notes |
|---|---|---|---|---|
| E1 | Image | “London Tower Bridge 22.jpg” | https://commons.wikimedia.org/wiki/File:London_Tower_Bridge_22.jpg | Includes geotag/camera location on page |
| E2 | Video | “LondonTowerBridge1998Video1.ogv” | https://commons.wikimedia.org/wiki/File:LondonTowerBridge1998Video1.ogv | CC BY-SA licensed clip |
| E3 | Reference | Tower Bridge background (structure/type) | https://en.wikipedia.org/wiki/Tower_Bridge | Used only as general reference |

---

## Reproducible Query Examples
- `"twin towers bridge walkway bascule" london`
- `site:commons.wikimedia.org Tower Bridge ogv`
- `Tower Bridge coordinates 51.503288 -0.073905`
- `reverse image search (keyframe / screenshot from E2)`

---

## Portfolio Note
This case study is designed to show a clean geolocation method with transparent sourcing and safe handling. No private data was collected or inferred.
