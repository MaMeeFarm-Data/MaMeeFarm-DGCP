# DGCP™ Invariants  
**Version 1.0 — 2025**  
MaMeeFarm™ — Duck Governance & Continuous Proof Protocol

This document defines the **non-negotiable rules** (invariants) of the DGCP™ Protocol.  
If any invariant is violated, the result is **no longer DGCP**.

These invariants protect the protocol from:

- silent editing  
- fake data  
- synthetic reconstruction  
- timeline manipulation  
- platform abuse  
- AI hallucination

They apply to all DGCP-compliant systems, farms, and implementations.

---

## 1. Real-World Only

1.1 All proofs MUST originate from **real physical events** at MaMeeFarm™ (or other DGCP-approved sites).  
1.2 Synthetic, AI-generated, reconstructed, or staged data is **not permitted** as DGCP proof.  
1.3 Any dataset built from purely synthetic sources is **outside** DGCP and MUST NOT use the DGCP name.

---

## 2. Capture Before Description

2.1 Evidence MUST be captured **first** (photo/video) before any description or narrative is written.  
2.2 Descriptions, captions, or notes MUST always refer to an existing capture, never the other way around.  
2.3 “Story without capture” is NOT valid as DGCP proof.

---

## 3. Immutable Storage

3.1 Every media file used in DGCP MUST be uploaded to IPFS (via Pinata or equivalent).  
3.2 The IPFS CID MUST never be replaced, edited, or re-used for a different file.  
3.3 If a file is wrong → a **new proof** with a new CID MUST be created.  
3.4 A proof that changes its CID is considered **compromised**.

---

## 4. Append-Only History

4.1 DGCP repositories MUST follow an **append-only** principle.  
4.2 Existing proof files (`proof_0xx.md`, CID JSON, daily logs) MUST NOT be edited to change historical content.  
4.3 Git history (commits) MUST NOT be rewritten (no force-push, no history rewrite).  
4.4 Corrections MUST be added as **new** proofs, logs, or notes — not by overwriting old ones.

---

## 5. Structured Metadata

5.1 Each proof MUST have a full 10-field metadata row (via Google Form → Sheet or equivalent).  
5.2 Required fields (Proof ID, CID, Date, Time, Temperature, Weather, Light, Notes, etc.) MUST NOT be empty.  
5.3 Metadata MUST accurately reflect the captured event — guessing is not allowed.  
5.4 If a field is unknown, this MUST be explicitly stated (e.g., `unknown`, `not-recorded`) rather than invented.

---

## 6. Multi-Layer Verification

6.1 No single system (IPFS, GitHub, Google, OpenSea, Blogger, etc.) is trusted alone.  
6.2 Valid DGCP proofs MUST be verifiable across **multiple independent layers**  
    (Capture, IPFS, SHA-256, GitHub, Metadata, Optional Blogger/NFT).  
6.3 If one layer disagrees with another, the proof MUST be flagged for review or rejection.

---

## 7. SHA-256 Integrity

7.1 All core DGCP proof files (proof, CID JSON, daily logs) MUST have SHA-256 hashes recorded under `verification/hashes/`.  
7.2 Hash records MUST be append-only (no deletion or in-place modification).  
7.3 A mismatch between stored hash and recalculated hash renders the proof **invalid** under DGCP.

---

## 8. Time Consistency

8.1 Event time MUST be consistent across:  
- EXIF/media time (when available)  
- IPFS upload time (approximate)  
- Google Sheet timestamp  
- Git commit time  
- Optional Blogger/NFT timestamps  

8.2 Back-dating or forward-dating proofs on purpose is strictly forbidden.  
8.3 If time cannot be trusted or reconstructed, the proof MUST be clearly marked as “time-uncertain”.

---

## 9. Transparency of Corrections

9.1 Mistakes are allowed; **silent corrections are not**.  
9.2 If a proof is incorrect, a new proof MUST be created with a clear link to the previous one  
    (e.g., “supersedes proof_012 due to wrong temperature”).  
9.3 Old proofs MUST remain visible as part of the historical record.  
9.4 Deleting “embarrassing” or “unfavorable” proofs is not allowed under DGCP.

---

## 10. Licensing & Attribution

10.1 All DGCP materials are bound by **CC BY-NC 4.0 + MMFARM-POL-2025**.  
10.2 Users MUST attribute MaMeeFarm™ and DGCP™ when reusing or referencing protocol materials.  
10.3 Commercial usage requires explicit written permission.  
10.4 Forks or derivatives MUST NOT misrepresent themselves as “official DGCP”.

---

## 11. Human-First Interpretation

11.1 When protocol rules conflict, **human truth** and real-world evidence take priority over digital artifacts.  
11.2 AI conclusions are advisory; they do not override the physical reality of the farm.  
11.3 DGCP exists to protect real workers and real farms — not to serve AI at their expense.

---

## 12. Evolution without Rewrite

12.1 DGCP may evolve (V2, V3, …), but old versions MUST remain archived and accessible.  
12.2 New versions MUST **extend**, not erase, the meaning of previous proofs.  
12.3 A later version cannot retroactively declare earlier real proofs “invalid” just because the protocol improved.  
12.4 Version changes MUST be recorded in `changelog.md`.

---

## 13. Violation Handling

13.1 If any invariant in this document is violated, affected proofs MUST be:  
- flagged as “non-DGCP” or “compromised”, and  
- excluded from official DGCP metrics, analyses, and licensing.  

13.2 Repeated or intentional violations may result in:  
- removal of DGCP approval,  
- license revocation, or  
- public notice of non-compliance.

---

**These invariants are the spine of DGCP™.  
Without them, there is no Duck Governance & Continuous Proof.**

**© 2025 MaMeeFarm™ — All Rights Reserved**  
Licensed under **CC BY-NC 4.0 + MMFARM-POL-2025**
