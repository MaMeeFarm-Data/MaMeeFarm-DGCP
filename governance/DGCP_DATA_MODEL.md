# DGCP™ Data Model — Real-Work Data (RWD) Structure (v1.0.0)
**License: MMFARM-POL-2025**  
**Data Governance & Continuous Proof™**

The DGCP™ Data Model defines how Real-Work Data (RWD) is structured, layered, and linked across the Proof Chain:  
**Human → Metadata → IPFS CID → GitHub SHA256 → DLT Timestamp**

This file establishes the canonical representation of RWD inside the DGCP protocol.

---

# 1. Purpose of the Data Model
The Data Model guarantees:

- **Authenticity:** Data originates from human intention  
- **Integrity:** Data cannot be modified after submission  
- **Traceability:** Every proof is linkable through SHA256 + CID  
- **Simplicity:** Zero IoT, zero sensor ingestion, zero biometric capture  
- **Global auditability:** Anyone can verify the entire chain  

The Data Model is intentionally minimal to protect workers and maximize verifiability.

---

# 2. Core Architecture of Real-Work Data (RWD)
Layer 1 — Core Proof Layer
Layer 2 — Context Layer
Layer 3 — Integrity Chain Layer

RWD consists of **three layers**:

Each layer has a specific role and scaling behavior.

---

# 3. Layer 1 — Core Proof Layer
The Core Proof is the **heart** of RWD.

| Field | Type | Purpose | Criticality |
|------|------|---------|-------------|
| `ipfs_cid_primary` | CIDv1 | Immutable proof artifact (photo/video) | Machine-Critical |
| `proof_id` | UUID | Unique identifier | Machine-Critical |
| `worker_id_public` | Public Key | Human-origin authentication | Machine-Critical |
| `signature` | Cryptographic | Signs entire metadata | Machine-Critical |
| `dms_version` | String | Enforces schema standard | Machine-Critical |

**Role:**  
Guarantee that the proof **originated from a human** and is **cryptographically sealed**.

---

# 4. Layer 2 — Context Layer
This represents the “human meaning” of the proof.

| Field | Type | Purpose | Notes |
|------|------|---------|------|
| `timestamp_local` | ISO8601 | Worker’s local time | Human-Interpretive |
| `location_label` | String | Coarse location (privacy-preserving) | Human-Interpretive |
| `work_type` | String | Category of work | Human-Interpretive |
| `short_human_description` | String | Worker’s voice and intent | Human-Interpretive |
| `tags` | Array | Optional context labels | Human-Interpretive |
| `ipfs_cid_additional` | Array | Optional supporting media | Human-Interpretive |

**Role:**  
Guarantee the **meaning**, **story**, and **context** behind each proof.

---

# 5. Layer 3 — Integrity Chain Layer
This layer links the proof into the DGCP Proof Chain.

| Field | Type | Purpose | Criticality |
|------|------|---------|-------------|
| `timestamp_utc` | ISO8601 | Global ordering | Machine-Critical |
| `git_commit_sha256` | SHA256 | Append-only provenance | Machine-Critical |
| `git_repo_url` | URL | Public registry endpoint | Machine-Critical |
| `ots_timestamp_ref` | String | Minimal DLT anchor | Machine-Critical |

**Role:**  
Guarantee the **immutability** and **public verifiability** of the entire historical chain.

---

# 6. Data Flow (Human → Global Registry)

[1] Worker Action
↓
[2] Capture Media (Phone)
↓
[3] Create Metadata (DMS v1.0.0)
↓
[4] Sign metadata (worker_id_public)
↓
[5] Upload proof to IPFS → CID
↓
[6] Commit metadata to GitHub (SHA256)
↓
[7] Daily SHA256 root timestamped on minimal DLT (Bitcoin/OTS)


This flow ensures each proof is:

- Human-origin  
- Immutable  
- Public  
- Timestamped  
- Globally auditable  

---

# 7. Data Model Philosophy

## 7.1 Minimalist by Design
DGCP does **not** allow:
- IoT ingestion  
- Biometric capture  
- Automated ML scoring  
- Surveillance-based data capture  

These violate DGCP Human-First principles and create power imbalances.

## 7.2 Human-First Interpretation
Machines validate structure.  
Human groups validate meaning.

## 7.3 Future-Proof & Versioned
The Data Model will evolve via:
- `dms_version`  
- Backward-compatible extensions in the Human-Interpretive fields

No version will break historical proofs.

---

# 8. Relation to Other DGCP Components

| Component | Relationship to Data Model |
|----------|----------------------------|
| DMS_SPEC.md | Defines the exact schema for each field |
| GOVERNANCE_MODEL.md | Defines who interprets meaning and resolves conflicts |
| VALIDATOR_SPEC.md | Defines machine-level structural checks |
| SCALING_ARCHITECTURE.md | Defines how RWD scales to 10,000 workers |
| MINIMAL_DLT_ANCHOR.md | Defines the timestamp anchoring method |

The Data Model is the **bridge** connecting all other components.

---

# Footer
**License: MMFARM-POL-2025**  
**DGCP™ — Data Governance & Continuous Proof™**

