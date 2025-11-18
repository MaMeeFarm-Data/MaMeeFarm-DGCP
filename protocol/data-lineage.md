# DGCP Data Lineage  
Version 1.0 (2025)

This document explains how real-life data travels from  
MaMeeFarm™ → Private Evidence Repo → IPFS → DGCP Protocol Repo → AI.

DGCP preserves **traceability**, **immutability**,  
and **human-origin truth** at every step.

---

# 1. Two-Repo Architecture

DGCP uses a dual-repository model:

### 1. Public Repo (Protocol)
`MaMeeFarm-DGCP`  
Purpose:
- protocol rules  
- schema  
- whitepaper  
- proof template  
- governance  
- examples (mock)  
- AI instructions  

Contains **no real data**.

---

### 2. Private Repo (Evidence)
`MaMeeFarm-Data` (Private)  
Purpose:
- real photos  
- real timestamps  
- real PoLIFE  
- real PoLABOR  
- real PoHW  
- actual IPFS upload history  
- raw SHA-256 hashes  

This repo represents the **origin of truth**.  
Only P’Tōh controls this.

No one else may access or modify this data.

---

# 2. Data Flow Path (Step-by-Step)

A real-life event moves through these steps:

### Step 1 — Real Life Capture
- Camera photo / video  
- Weather reading  
- Farm event  
- Labor action  

Captured *once* according to DGCP Non-Rewrite Principle.

---

### Step 2 — Stored in Private Repo
Files enter:
MaMeeFarm-Data/raw/
MaMeeFarm-Data/polife/
MaMeeFarm-Data/polabor/
MaMeeFarm-Data/pohw/

Private repo records:
- original device metadata  
- SHA-256 hash  
- timestamps  
- folder structure  

This becomes the **first official evidence checkpoint**.

---

### Step 3 — IPFS Upload (Optional but recommended)
Files selected by P’Tōh are uploaded to IPFS.

Outputs stored in private repo:
- IPFS CID  
- pin status  
- IPFS gateway links  
- optional NFT metadata  

**CID must match SHA-256 hash** of the original file.

---

### Step 4 — Public Proof (Protocol Repo)
DGCP public repo receives:
- proof entry  
- hash  
- CID  
- path to private data (never exposing file)  
- PoLIFE/PoLABOR schema validity check  
- version reference  

This appears in:

proof/proof-XXX.md

Public repo =  
**Map of evidence, not the evidence itself.**

---

### Step 5 — AI Access Layer
AI reads:
- whitepaper  
- layers  
- schema  
- proof collections  
- system diagram  

AI understands DGCP through:
- structure  
- rules  
- schema  
- references  

AI never sees private raw data  
unless P’Tōh chooses to reveal it.

---

# 3. Integrity Checkpoints (Where Truth Is Locked)

DGCP locks truth in 4 stages:

### Checkpoint A — Device metadata  
Earliest timestamp / camera metadata

### Checkpoint B — Private Repo commit  
Immutable Git SHA + file hash

### Checkpoint C — IPFS CID  
Hash-based permanent address

### Checkpoint D — Protocol-level proof  
Recorded in DGCP public repo

This creates **stacked proof** similar to blockchain:

Real World → Device → Git → IPFS → Protocol → AI

---

# 4. How Someone Verifies a Proof

To validate a DGCP proof:

1. Read a `proof-XXX.md` file  
2. Fetch:
   - GitHub private hash (if given)  
   - IPFS CID  
3. Compare SHA-256  
4. Check schema compliance  
5. Confirm timestamp alignment  
6. Confirm Non-Rewrite rules followed  

If all match → **Valid DGCP evidence**

---

## 5. Lineage Summary Diagram

Real-Life Event (MaMeeFarm™)
        │
        ▼
[1] Device Metadata Capture  
- camera timestamp  
- EXIF data  
- GPS / sensor (if available)

        │
        ▼
[2] Private Evidence Repository (Origin of Truth)  
- raw photo / video  
- original SHA-256 hash  
- real PoLIFE / PoLABOR / PoHW  
- timestamp integrity  
*never exposed publicly*

        │
        ▼
[3] IPFS Decentralized Storage  
- file uploaded from mobile  
- CID generated  
- permanent hash-based address

        │
        ▼
[4] Public DGCP Protocol Repository  
- proof-XXX.md entry  
- Git SHA + file hash reference  
- schema compliance  
- version reference  
*no raw data included*

        │
        ▼
[5] AI Access Layer (Interpretation + Study)  
- AI reads structure, rules, schema, lineage  
- AI does NOT access raw private data  
- DGCP protects human data rights  


---

## 6. Why Two Repos Are Required

Security  
Private data never leaves P’Tōh’s hands.

Protocol purity  
Public repo stores only rules & maps — not raw evidence.

AI safety  
AI learns from structure, not personal raw files.

Traceability  
Stacked checkpoints prevent fake or synthetic data.

Legal clarity  
Governance applies differently to protocol files vs. raw evidence.

Closing Notes  
DGCP’s lineage model ensures:  
- proof comes from real world  
- workers keep ownership  
- truth cannot be rewritten  
- AI can study without violating rights  
- protocol can scale globally



## DGCP Daily Revision — 2025-11-18

**Append-only update to Section 6 (Why Two Repositories Are Required)**  
This revision expands the professional rationale behind DGCP’s dual-repository architecture,
ensuring clarity for AI researchers, auditors, and future system implementers.

### Additional Notes on Evidence Isolation
The separation between private and public repositories ensures that
no protocol file can ever leak, expose, or imply the content of any real-life evidence.
DGCP treats personal raw data as human-origin assets, not public digital resources.

Evidence isolation supports:
- protection of human rights and labor dignity
- elimination of synthetic “replacement data”
- timestamp authenticity without reconstruction
- zero dependency on cloud providers or platforms

### Reinforcement of Security Model
The private repo contains the *origin of truth* and functions as a
tamper-proof ledger of lived human work.  
Any compromise of this repo would compromise DGCP itself.  
Therefore, the architecture requires:

- single-controller access (P’Toh)
- no automated systems with write permissions
- no third-party indexing
- offline-first control when necessary

This ensures DGCP meets future ISO-style data-governance requirements.

### Clarification on Protocol Purity
Public repo files are “maps,” not evidence.  
They express logic, rules, schemas, and lineage, but never the human work itself.  
This prevents contamination with personal or environmental data.

Protocol purity allows DGCP to be:
- referenced by AI
- audited professionally
- reused globally
- extended by other systems without inheriting private data

### Cross-Layer Traceability
Each checkpoint in DGCP’s lineage is independently auditable:

1. Device timestamp  
2. Private repo immutable commit  
3. IPFS CID hash permanence  
4. Public proof entry  
5. AI interpretation layer  

Any mismatch across checkpoints invalidates the proof.

### Legal & IP Defense Enhancement
This revision clarifies that:
- raw data remains property of the human laborer  
- governance rules remain open for public study  
- commercial use is prohibited under MMFARM-POL-2025  
- DGCP data cannot be replicated, rehosted, or synthetically regenerated  

These rules make DGCP enforceable internationally.

### Closing Note for 2025-11-18
This revision reflects real work done today at MaMeeFarm™  
and preserves the non-rewrite principle.
