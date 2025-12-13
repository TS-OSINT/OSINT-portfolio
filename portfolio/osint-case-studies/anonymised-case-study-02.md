# Anonymised OSINT Case Study 02 – Online Narrative & Claim Verification

All case studies are fully anonymised and created for portfolio purposes only.
No private, confidential or non-public information is included.

## Summary
This case study demonstrates a practical, entry-level OSINT workflow for verifying a circulating online claim and mapping how the narrative spread across platforms. The goal is to show clear methodology and documentation, not to “expose” a specific person or group.

## Scenario (Anonymised)
A public claim began circulating online about a “new policy change” affecting a local community. The claim spread rapidly through reposts and screenshots, with conflicting versions of the alleged statement.

## Objectives
1. Verify whether the claim is accurate.
2. Identify the earliest available source of the claim.
3. Map the spread of the narrative across platforms.
4. Document findings in a transparent, reproducible way.

## Scope and Safety
- Only publicly accessible information was used.
- No attempt was made to identify private individuals.
- No doxxing, harassment, or contact with subjects.
- Personal identifiers and unique details have been removed.

## Tools and Sources Used (Open)
- Search engines and advanced operators (site:, filetype:, exact match quotes)
- Web archives (e.g., cached pages / archived snapshots where available)
- Public official sources (government/organisation websites and press pages)
- Public social platforms (public posts only)
- Reverse image search for screenshots (when applicable)
- Basic timeline tracking in a spreadsheet

## Workflow and Findings (High-Level)

### 1. Claim capture and normalization
- Copied key claim text into a notes file.
- Listed variations of the claim wording (to catch paraphrases).
- Captured post dates/times as displayed and noted time zone uncertainty.

Output: A “Claim Statement” section with 3–5 wording variants.

### 2. Source tracing (earliest known mention)
- Searched exact-match claim fragments in quotes.
- Used platform search plus Google/Bing queries.
- Looked for the earliest timestamped post that contained the full claim text.

Finding: The earliest public mention located was a post that referenced a screenshot, not an original document. This suggested the claim likely originated elsewhere.

### 3. Screenshot / document verification
- Reverse searched the screenshot to detect reuse.
- Checked for signs of editing (cropping artifacts, mismatched fonts, missing headers).
- Attempted to find an original statement on official pages and press releases.

Finding: No matching original statement was found on official sources for the date range referenced. Multiple reposts used the same screenshot with slightly different captions.

### 4. Corroboration against authoritative sources
- Checked the relevant authority’s website, press pages, and archived versions.
- Looked for policy updates, FAQs, official statements, or meeting minutes.
- Compared the claim wording to known official terminology.

Finding: Official documentation available publicly did not support the specific wording in the screenshot. The closest official information described a different process than the claim suggested.

### 5. Narrative spread mapping (basic)
- Collected a small sample of public posts (e.g., 20–40) across platforms.
- Recorded: date/time, platform, post type (original/repost), and whether it referenced the screenshot.
- Noted amplification by a small number of accounts and pages.

Finding: The narrative spread followed a screenshot-first pattern. A few high-engagement reposts accelerated reach, while later posts added interpretation rather than new evidence.

## Conclusion (Careful wording)
Based on the open sources reviewed, the claim could not be verified as presented. The available public official information did not match the alleged statement, and the screenshot appeared repeatedly without a traceable original source. The most likely explanation is that the claim was based on a misinterpretation, an outdated reference, or an edited/unsupported screenshot.

## What I Would Improve Next Time
- Expand the dataset size and standardise timestamps.
- Add more rigorous link analysis (where available).
- Create a clearer evidence log with hashes for key screenshots.
- Build a repeatable template for claim verification and narrative tracking.

## Appendix – Reproducible Query Examples (Generic)
- "exact phrase from the claim"
- site:officialdomain.tld "keyword"
- filetype:pdf site:officialdomain.tld policy update
- "keyword" "date" "press release"
