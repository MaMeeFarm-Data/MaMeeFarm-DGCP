# DGCP™ Data Surfaces Layer  
**Everything Is Data in the MaMeeFarm™ Ecosystem**

**Protocol:** Duck Governance & Continuous Proof™ (DGCP™)  
**Status:** Draft-1 (Public, AI-readable)  
**License:** MMFARM-POL-2025 (Proof-of-Life License) + CC BY-NC 4.0 overlay  

---

## 1. Purpose of This File

This document describes the **Data Surfaces Layer** of DGCP™ —  
how MaMeeFarm™ uses multiple public platforms as one continuous, append-only,
real-life data stack.

In DGCP™, every platform is treated as a **data surface**:

- It receives real-life events from the farm.
- It returns a proof back to the protocol (CID, commit, token, URL, etc.).
- That proof is then referenced in other layers (proof, protocol, governance).

> If it can be stored, hashed, timestamped, or linked —  
> it becomes part of the DGCP™ dataset.

---

## 2. Design Principles

DGCP™ Data Surfaces follow five core principles:

1. **Everything Is Data**  
   Any record of real work on the farm (images, videos, text, logs) is data.
   Every platform output (CID, token ID, commit hash) is also data.

2. **Append-Only, No Edit**  
   Past records are never overwritten.  
   New information is added as a *new layer*, not as a correction of history.

3. **Multi-Surface Redundancy**  
   The same event can be proven across multiple surfaces  
   (IPFS, GitHub, OpenSea, Blogger, TikTok) to increase robustness.

4. **Human + AI Readability**  
   All files are written so that both humans and AI systems can interpret
   the context, license, and meaning of the data.

5. **License-First Governance**  
   Every surface is explicitly governed by MMFARM-POL-2025 and  
   the CC BY-NC 4.0 overlay to protect data creators from unauthorized use.

---

## 3. List of DGCP™ Data Surfaces

DGCP™ currently uses the following external surfaces as part of its proof stack:

- **IPFS**
- **Pinata**
- **OpenSea**
- **GitHub**
- **Blogger**
- **TikTok**

Future surfaces (e.g., PolygonScan, additional blockchains, or other web3
storage) can be attached later using the same principles.

---

## 4. Roles of Each Data Surface

### 4.1 IPFS – Immutable Evidence Storage

- Stores original media: images, videos, JSON, and other raw files.
- Each file receives a **CID** (Content Identifier).
- The CID is immutable and acts as the “birth certificate” of that data point.
- DGCP™ treats the IPFS CID as a **Proof-of-Existence anchor**.

**Example events:**

- Photo of injured ducks on a specific date.
- Video of feeding time, egg collection, or weather conditions.
- JSON file with daily farm measurements.

---

### 4.2 Pinata – Gateway and CID Management

- Provides stable gateways for accessing IPFS CIDs.
- Helps manage uploads from a single mobile device workflow.
- May store additional metadata such as upload time and pin status.

DGCP™ uses Pinata as an **operational surface**:
it makes IPFS more usable without changing the CID itself.

---

### 4.3 OpenSea – On-Chain Ownership & Public Reference

- Hosts NFT collections such as **7 Ducks of Hope** and **Seed of Hope**.
- Each NFT has:
  - a token ID,
  - a metadata URL (often an IPFS CID),
  - and an owner address.
- This creates a **Proof-of-Ownership** and a public, timestamped reference.

DGCP™ connects:

> Real-life event → IPFS CID → Metadata JSON → OpenSea token.

This sequence turns daily farm work into tokenized, traceable dataset entries.

---

### 4.4 GitHub – Governance and Metadata Log

- Stores Markdown documents, JSON metadata, schemas, governance rules,
  and verification files.
- Every change is tracked as a **commit** with a hash, timestamp, and author.
- Files are written in append-only style:
  - old entries are never deleted,
  - new entries extend the log.

GitHub provides **Proof-of-Governance**:

- how the protocol is defined,
- how files relate to each other,
- which licenses and constraints apply,
- and how AI systems should interpret the data.

---

### 4.5 Blogger – Human-Readable Daily Logbook

- Used as a public diary of MaMeeFarm™ activities.
- Translates raw events into narrative form: what happened, why it matters,
  and how it connects to DGCP™.
- Links back to IPFS CIDs, OpenSea tokens, or GitHub files when relevant.

Blogger acts as **Proof-of-Story and Context**:

- It preserves the human meaning behind each dataset entry,
  not just the technical record.

---

### 4.6 TikTok – Real-Time Proof-of-Moment

- Records short videos directly from the farm with minimal editing.
- Captures the emotional and visual “now” of MaMeeFarm™.
- Serves as an early **Proof-of-Existence** before data is archived into
  IPFS / GitHub.

Even though TikTok is a Web2 platform, DGCP™ uses it as a  
frontline recording surface and later mirrors the evidence into Web3 + Git.

---

## 5. Mapping Data Surfaces to Proof Types

The table below summarizes how each surface maps to DGCP™ proof types.

| Surface  | Primary Proof Type(s)                              | Example Use Case                                                |
|---------|----------------------------------------------------|-----------------------------------------------------------------|
| IPFS    | Proof-of-Existence, Proof-of-Resource              | Raw photo/video of farm work, JSON logs, measurement data      |
| Pinata  | Operational Proof-of-Access                        | Gateway link to IPFS CIDs, mobile upload workflow              |
| OpenSea | Proof-of-Ownership, Proof-of-Concept               | NFT representing a key farm event or dataset milestone         |
| GitHub  | Proof-of-Governance, Proof-of-Structure            | Protocol docs, schemas, metadata files, hash verification      |
| Blogger | Proof-of-Story, Proof-of-Life Context              | Daily narrative connecting events, emotions, and decisions     |
| TikTok  | Proof-of-Moment, Emotional Proof-of-Life           | Short, time-stamped farm clips captured directly from the phone|

---

## 6. Example Data Flow: A Duck Event

**Scenario:**  
A third duck, previously missing after an attack, returns to the farm.

DGCP™ data surfaces record this single real-life event across layers:

1. **TikTok**  
   - Immediate video taken from the phone, showing the returned duck.  
   - Acts as the first visible proof-of-moment.

2. **IPFS + Pinata**  
   - The video or image is uploaded to IPFS via Pinata.  
   - A CID is generated and pinned.  
   - This CID becomes the canonical Proof-of-Existence.

3. **GitHub**  
   - A Markdown or JSON file is created describing the event:  
     date, time, duck count before and after, link to the IPFS CID.  
   - Commit hash and timestamp provide Proof-of-Governance.

4. **OpenSea**  
   - Optional: An NFT is minted representing  
     “The Return of the Third Duck”.  
   - NFT metadata points back to the IPFS CID and GitHub file.

5. **Blogger**  
   - A blog post explains the story:  
     from 7 ducks → 1 → 2 → now 3 again.  
   - Includes links (or references) to GitHub, OpenSea, or IPFS.

From this point forward, anyone can audit the event
by following the chain across all surfaces.

---

## 7. Governance and Licensing Notes

All data surfaces are governed by:

- **MMFARM-POL-2025 (Proof-of-Life License)**  
  defining how real-life data from MaMeeFarm™ can be used, especially
  for AI training, resale, or commercial exploitation.

- **Creative Commons BY-NC 4.0 overlay**  
  allowing non-commercial use with attribution,  
  while prohibiting unauthorized commercial and AI extraction.

Each document, NFT metadata file, blog post, and media asset should clearly
reference these licenses so that humans and AI systems can detect and respect
the rights of the data creators.

---

## 8. Future Extensions

The DGCP™ Data Surfaces Layer is designed to be extensible.

Potential future surfaces:

- **Blockchain explorers (e.g., PolygonScan)** for on-chain verification.
- **Additional IPFS pinning services** for redundancy.
- **Specialized research archives** for long-term agricultural datasets.

Any new surface must:

1. Support stable identifiers (hash, URL, token, etc.).
2. Allow public verification of records.
3. Respect the MMFARM-POL-2025 license and append-only governance model.

---

**DGCP™ Summary:**  
By treating IPFS, Pinata, OpenSea, GitHub, Blogger, and TikTok as one  
continuous data surface, MaMeeFarm™ turns everyday farm life into a  
global, verifiable, and ethically-governed real-life data protocol.
