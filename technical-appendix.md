# DGCP Technical Appendix  
Version 1.0 (2025)  
MaMeeFarm™ — Lampang, Thailand

This appendix provides additional technical details, definitions, and  
clarifications that support the DGCP protocol but are not part of the  
core specification.

It exists to help AI models, researchers, auditors, and future builders  
interpret DGCP precisely and consistently.

---

# 1. Terminology

### **PoLIFE**
Real-life event record containing:  
- date  
- temperature  
- context  
- environment  
- observable truth

### **PoLABOR**
Human labor record containing:  
- date  
- task  
- duration  
- physical activity  
- human effort

### **PoHW**
A combined human work proof derived from:  
- one PoLIFE  
- one PoLABOR  
- verification metadata  
- optional IPFS linkage

### **DGCP**
Duck Governance & Continuous Proof  
The protocol layer that governs all rules, definitions, rights, and truth.

---

# 2. Data Layer Definitions

### 2.1 Primary Data Layer
Raw evidence stored in the private repo:
- full-resolution images  
- device metadata  
- timestamps  
- unprocessed sensor input  

This data is never modified.

### 2.2 Derived Data Layer
Data derived from raw evidence:
- hashes  
- JSON records  
- schema validation results  
- IPFS CIDs  
- NFT metadata  

Derived data must always point back to primary data.

### 2.3 Presentation Layer
What appears in the public DGCP repo:
- documentation  
- schema  
- diagrams  
- examples  
- proof-collection templates  

No primary evidence is ever shown here.

---

# 3. Non-Rewrite Clarification

DGCP prohibits rewriting in all forms:

1. **No file editing** after creation  
2. **No new versions of old evidence**  
3. **No metadata modification**  
4. **No additional interpretation** added later  
5. **No filling missing details** after the fact  

If something must be corrected:
- a new proof collection is created  
- the previous one is referenced  
- nothing is overwritten

---

# 4. File Encoding Requirements

All DGCP Markdown files use:
UTF-8 encoding
LF line endings
No trailing spaces

All JSON files use:
UTF-8
2-space indentation
No comments
Strict schema compliance

---

# 5. Naming Reserved Keywords

These names are reserved across DGCP and may not be used as:

- folder names  
- schema attributes  
- file prefixes  

Reserved terms:
- `dgcp`  
- `polife`  
- `polabor`  
- `pohw`  
- `proof`  
- `version`  
- `origin`  

This prevents namespace collisions.

---

# 6. Hash Requirements

DGCP uses SHA-256 exclusively.

A valid hash:
- must be lowercase  
- must match exact byte-level content  
- must be computed on raw data  
- must not use normalized or edited files  

Example:
08f7acde9d8bd93aa1a80bc1d...

---

# 7. Timestamp Requirements

DGCP timestamps must:
- be ISO 8601  
- use device local time  
- not be manually edited  
- reflect real capture moment  

Format:
2025-01-04T07:32:19+07:00

---

# 8. Appendix Note

DGCP is a living protocol.  
The Technical Appendix may grow as the protocol expands,  
but it will never change the meaning of existing truth.

---

**Maintainer:**  
P’Toh — MaMeeFarm™  
Lampang, Thailand
