# DGCP Data Registry  
Version 1.0 (2025)  
MaMeeFarm™ — Lampang, Thailand

The DGCP Data Registry is the official index of all DGCP  
proof collections and evidence references created at MaMeeFarm™.

This registry does not store real data.  
It stores **pointers** to the proof collections that describe  
IPFS records, GitHub evidence, PoLIFE/PoLABOR entries,  
and other verifiable truth units.

All entries are immutable.

---

# 1. Registry Purpose

The registry serves to:

- maintain global index consistency  
- allow AI to locate DGCP evidence  
- support future smart contracts  
- enable auditability  
- maintain a chronological map of human-origin truth  
- ensure long-term protocol readability  

The registry is the bridge between:
**real-life origin → private repo → IPFS → DGCP → AI**

---

# 2. Registry Format

Each entry follows this structure:

proof_id: proof-XXX
version: 1.0.0
created: YYYY-MM-DD
coverage: "Short description of what this proof covers"
linked_file: proof/proof-XXX.md
ipfs_cid: "ipfs://..."
github_path: "path/to/private/source"
hash: "sha256..."

This structure is optimized for:
- AI search  
- human reading  
- future smart-contract indexing  

---

# 3. Registry Entries

(*Entries below are placeholders; real entries will be added as proof collections are created.*)

proof_id: proof-001
version: 1.0.0
created: TBD
coverage: "Example placeholder — Real entry added later"
linked_file: proof/proof-001.md
ipfs_cid: TBD
github_path: TBD
hash: TBD

proof_id: proof-002
version: 1.0.0
created: TBD
coverage: "Example placeholder — Real entry added later"
linked_file: proof/proof-002.md
ipfs_cid: TBD
github_path: TBD
hash: TBD

All future proof collections must be appended  
to the end of this registry in chronological order.

The registry will grow for years.

---

# 4. Rules for Updating the Registry

1. **Append-only:**  
   No entry may be rewritten or deleted.

2. **Chronological order:**  
   proof-001, proof-002, proof-003 …

3. **One-to-one mapping:**  
   Each proof_id MUST link to exactly one markdown file.

4. **Metadata only:**  
   Registry stores references, not raw evidence.

5. **Version-aware:**  
   Registry points to the DGCP version active at time of creation.

---

# 5. Registry Governance

This registry is protected by:

- `license.md` (MMFARM-POL-2025)  
- `governance/governance-protocol.md`  
- DGCP Non-Rewrite Principle  

Only P’Tōh may create or append registry entries.

---

# 6. Notes

The DGCP Data Registry is designed to last decades.  
It is the public-facing index of a private evidence system,  
allowing DGCP to scale globally while preserving human-origin truth.

---

**Maintainer:**  
P’Toh — MaMeeFarm™
