# DGCP™ Governance — Traceability Specification  
Version: 1.0.0  
Status: Draft  
License: MMFARM-POL-2025

## 1. Overview  
Traceability is the core governance requirement of the DGCP™ (Data Governance & Continuous Proof™) system.  
Every Proof generated at MaMeeFarm™ must be verifiable across **all layers** without relying on trust, interpretation, or central authority.

This specification defines the minimum rules for **cross-layer traceability**, covering IPFS, GitHub, JSON metadata, Daily Logs, and Narrative Layers.

---

## 2. Traceability Principles  

### 2.1 Cross-Layer Link Architecture  
Each Proof must link across these layers:

1. **Raw Media Layer (IPFS CID)**
2. **Hash Layer (SHA-256 in GitHub)**
3. **Metadata Layer (JSON)**
4. **Narrative Layer (Markdown)**
5. **Governance Layer (DGCP Specs)**

A break or mismatch in any layer means the Proof is invalid.

---

### 2.2 Immutable Origin  
- The original CID is the source of truth.  
- No replacement images, no edits, no filters, no regeneration.  
- If the file is corrupted or missing, the Proof must be marked “Compromised”.

---

### 2.3 Human-Context Linking  
Every Proof must reference the “Real-Work Context” recorded that day:
- Weather  
- Time  
- Temperature  
- Location  
- Activity context  
- Who performed the work (MaMee or P’Toh)

---

## 3. Minimum Required Fields  

| Layer | Required Field | Example |
|------|----------------|---------|
| IPFS | `cid_original` | `bafy...` |
| GitHub | `sha256` | `12af...` |
| Metadata | `activity` | `Collected duck egg` |
| Narrative | `story` | “Today MaMee walked 3 km to buy food...” |
| Governance | `verification_rule` | “SHA256 must match GitHub log” |

---

## 4. Audit Rules  

1. CID → SHA must match metadata  
2. Metadata → Narrative must match daily-log facts  
3. Timestamp → must appear in at least 2 layers  
4. No synthetic data allowed  
5. No AI-generated media allowed  

---

## 5. Why Traceability Matters  
DGCP is designed for:
- AI research  
- Data integrity  
- Real-World Data certification  
- Anti-synthetic datasets  
- Proof-of-Human-Work (PHW)

Traceability is the only mechanism that allows the world to trust MaMeeFarm™ data without ever knowing MaMee personally.

---

## 6. Conclusion  
This Traceability Specification is a global-ready governance rule.  
It defines *how truth is anchored* inside DGCP and ensures every Proof can be verified decades into the future.
