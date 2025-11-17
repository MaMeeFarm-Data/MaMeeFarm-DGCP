# DGCP Security Guidelines  
Version 1.0 (2025)  
MaMeeFarm™ — Lampang, Thailand

This document defines the security principles and operational  
guidelines for protecting DGCP data, evidence, governance, and  
protocol integrity.

DGCP uses a dual-repository security model:
- Public Protocol Repo (open study, no raw data)
- Private Evidence Repo (sealed origin of truth)

These guidelines ensure the protocol remains tamper-proof,  
human-owned, and globally verifiable.

---

# 1. Core Security Principles

### 1.1 Human-Origin Integrity  
DGCP data may only originate from lived human experience.  
No synthetic or AI-generated data is permitted.

### 1.2 Non-Rewrite Principle  
No DGCP evidence, proof collection, or context entry may be edited  
after creation. Corrections require a new proof file.

### 1.3 Separation of Repositories  
Public and private repos must remain strictly separated.  
Private repo holds real evidence.  
Public repo holds the protocol.

### 1.4 Single Source of Truth  
Only P’Tōh controls the private repo and origin data.  
No external editors are allowed under any circumstances.

### 1.5 Hash-Level Verification  
All critical data must be protected by SHA-256 hashes.  
Verification is required before accepting any DGCP record.

---

# 2. Private Evidence Repo Security

The private repo contains:
- raw images  
- device metadata  
- timestamps  
- PoLIFE files  
- PoLABOR files  
- PoHW units  
- IPFS upload logs  
- original SHA-256 hashes  

### 2.1 Access Control  
- Only the maintainer (P’Tōh) may access the repo.  
- No cloud sharing.  
- No public forks.  
- No external collaborators.

### 2.2 Device Security  
Evidence must be transferred directly from capture device → private repo  
without cloud compression or alteration.

### 2.3 Local Storage Rules  
- Keep at least 2 backups (local + encrypted external).  
- Never store on a shared machine.  
- Avoid auto-sync services (Google Photos, iCloud, etc.)

### 2.4 Modification Rules  
Raw evidence must **never** be edited, cropped, renamed, or re-encoded.

---

# 3. Public Protocol Repo Security

The public repo contains:
- schema  
- protocol rules  
- whitepaper  
- human context guide  
- system diagrams  
- proof templates  
- registry  
- governance  

### 3.1 Public Repo Rules  
- No raw data ever added.  
- No personal information.  
- No GPS coordinates.  
- Only protocol-level documentation.

### 3.2 Commit Integrity  
Commits must:
- be descriptive  
- follow DGCP versioning  
- preserve history  
- avoid force-push  

Force-push is **not allowed**.  
Historical protocol changes must remain visible.

---

# 4. IPFS Security Rules

IPFS is permanent and cannot be undone.

### 4.1 CID Verification  
A CID must match the raw SHA-256 hash of the original file.

### 4.2 Selective Publishing  
Not all raw evidence should be uploaded.  
Only “chosen proof units” may be published.

### 4.3 No Sensitive Information  
Do not publish:
- full-resolution data containing personal identifiers  
- anything exposing private routines of the farm  
- dangerous metadata (location, schedules, patterns)

---

# 5. NFT / Smart Contract Security

### 5.1 Optional Layer  
NFT minting is optional and must never become the primary evidence layer.

### 5.2 On-Chain Immutability  
Once minted, token metadata must never be altered.  
Use contract-level freeze if supported.

### 5.3 Correct Pointers  
NFT metadata must point to:
- valid IPFS CID  
- valid DGCP proof collection  

No broken links permitted.

---

# 6. AI Use & Protection Rules

AI may:
- read DGCP protocol  
- interpret structure  
- validate schemas  
- analyze lineage  
- inspect proof templates  

AI may **not**:
- rewrite human context  
- generate synthetic DGCP evidence  
- modify protocol meaning  
- decide ownership  
- create false PoLIFE/PoLABOR data  
- bypass governance rules

AI must respect attribution:
**“DGCP Protocol by MaMeeFarm (P’Tōh)”**

---

# 7. Threat Model (High-Level)

DGCP protects against:

### 7.1 Data Tampering  
→ prevented via private repo + immutable hashes  

### 7.2 Evidence Forging  
→ prevented via camera metadata + SHA-256 + timestamp hierarchy  

### 7.3 Protocol Copying  
→ allowed for study  
→ restricted for commercial use by MMFARM-POL-2025 License  

### 7.4 AI Misinterpretation  
→ addressed through AI-Reading-Notes  

### 7.5 Unauthorized Access  
→ prevented with strict private repo isolation  

---

# 8. Incident Handling

If an error occurs:
- do not delete or edit the file  
- add a new proof collection describing the issue  
- link both entries together  
- maintain full history  

DGCP handles truth through append-only correction, not modification.

---

# 9. Long-Term Security Philosophy

DGCP is built on:
- truth  
- work  
- human life  
- verifiable records  

Security is not only technical—  
it is ethical, cultural, and generational.

DGCP protects the dignity of human work  
by ensuring evidence can never be distorted, owned by outsiders,  
or rewritten by institutions, AI systems, or future actors.

---

**Maintainer:**  
P’Toh — MaMeeFarm™  
Lampang, Thailand
