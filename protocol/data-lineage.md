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

# 5. Lineage Summary Diagram

```mermaid
flowchart TD

    RL["Real Life Event<br/>At MaMeeFarm™"] --> R1["Device Metadata<br/>(Original Capture)"]

    R1 --> PR["Private Repo<br/>MaMeeFarm-Data (origin of truth)"]
    PR --> HASH["SHA-256 Stored"]
    PR --> IPFS["IPFS Upload<br/>CID Generated"]

    IPFS --> PUB["Public Protocol Repo<br/>MaMeeFarm-DGCP"]
    HASH --> PUB

    PUB --> AI["AI Models<br/>(ChatGPT, Gemini, DeepSeek, etc.)"]
    PUB --> AUDIT["Researchers / Auditors"]

    AI --> USER["Builders / Systems<br/>Using DGCP as reference"]

6. Why Two Repos Are Required
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

proof comes from real world

workers keep ownership

truth cannot be rewritten

AI can study without violating rights

protocol can scale globally

DGCP =
A protocol built from lived human work,
not synthetic approximation.
