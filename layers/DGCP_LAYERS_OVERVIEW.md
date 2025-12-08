# DGCP Layers Overview

Version: 1.0.0  
MMFARM-POL-2025

---

## 1. Data Surface Layer (DSL)
The DGCP Data Surface Layer defines all externally exposed data planes that interact with the DGCP Proof Chain.

- IPFS (Primary content-addressable surface)
- Pinata / Web3.storage (Optional redundant pinning)
- GitHub Commits (Metadata registry, SHA-256 indexed)
- Minimal DLT Timestamp Surface (OTS / Bitcoin)

**Functions**
- Provides tamper-evident public data access
- Anchors metadata across surfaces
- Ensures multi-surface redundancy

---

## 2. Proof-of-Human-Work Layer (PoHW)
The PoHW layer ensures that all proofs originate from human action, not automated devices or AI systems.

**Invariants**
- Worker-signed metadata only
- No IoT ingestion
- No automated content generation
- Mandatory human description field
- Human-first auditability

**Outputs**
- Verified human-origin proof package
- Signed DMS object
- CID reference for immutable media

---

## 3. Labor Classification Layer (PoLABOR)
PoLABOR classifies the nature of the labor using controlled vocabulary categories.

**Categories**
- farm.work
- animal.care
- crop.lifecycle
- maintenance
- household.work
- energy.management

**Functions**
- Standardizes labor semantics
- Enables ethical analysis
- Preserves cross-regional interpretability

---

## 4. Life Context Layer (PoLIFE)
PoLIFE stores contextual information about the worker’s environment that influences proof interpretation.

**Components**
- Weather context (manual or observational)
- Environmental conditions
- Location label (coarse, non-PII)
- Daily-life conditions relevant to proof meaning

**Purpose**
- Preserves the human context of the proof
- Prevents dehumanized machine-only interpretation
- Strengthens fairness in analysis

---

## 5. Indexing Layer
Defines rules for indexing proofs across surfaces:

- Proof ID → CID → Commit SHA → Timestamp Anchor
- Reverse index: Commit → Proof Map → Human Context Map
- Public read-only schema for verifiable traversal

---

## 6. Governance Layer (Interface)
Defines which components of the layers are governed by:

- Machine validation only
- Human-only validation
- Shared federated review

Mapping:

| Layer | Machine-Critical | Human-Interpretive |
|-------|------------------|---------------------|
| DSL | Yes | No |
| PoHW | Yes | Yes |
| PoLABOR | No | Yes |
| PoLIFE | No | Yes |
| Indexing | Yes | No |
| Governance | No | Yes |

---

## 7. Layer Invariant Summary
Every DGCP layer must follow these core invariants:

1. Immutable  
2. Append-only  
3. Human-first  
4. Anti-fake  
5. Multi-surface  
6. Privacy-preserving  
7. Globally auditable  

---

## 8. Layer Output Contract
All layers output to the DGCP Minimal Proof Chain:

```
Human Action  
→ DMS Metadata  
→ IPFS CID  
→ GitHub Commit SHA  
→ Minimal DLT Timestamp
```

This is the canonical DGCP proof path for all future implementations.

---

MMFARM-POL-2025  
All rights reserved under dual-license terms.
