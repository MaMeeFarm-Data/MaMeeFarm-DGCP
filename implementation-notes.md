# DGCP Implementation Notes  
Version 1.0 (2025)  
MaMeeFarm™ — Lampang, Thailand

This document provides high-level implementation notes  
for anyone who wishes to adopt the DGCP model in their own environment.

It does **not** include any real data from MaMeeFarm.  
It only explains the structure, workflow, and system requirements  
to implement DGCP properly while respecting human-origin truth.

---

# 1. Who Can Implement DGCP?

DGCP may be implemented by:
- small farms  
- labor groups  
- families  
- independent workers  
- craft communities  
- researchers  
- decentralized data projects  

DGCP does **not** require high technology to start.  
It requires:
- honesty  
- consistency  
- traceability  
- human work  

The protocol is human-first.

---

# 2. Minimum Requirements

To implement DGCP, you need:

### Hardware:
- A mobile phone with a camera  
- A computer (optional, but recommended)
- External SSD or HDD for backups

### Software:
- GitHub account  
- A private repo for raw evidence  
- A public repo for your DGCP protocol implementation  
- IPFS pinning service of your choice  
- SHA-256 hashing tool (built into most OS)

### Skills:
- basic folder management  
- ability to write short notes  
- consistent daily discipline  

DGCP is designed for real workers, not engineers.

---

# 3. Two-Repo Requirement

DGCP requires:
1. **Private Evidence Repo**  
   - holds raw photos  
   - holds device metadata  
   - holds timestamps  
   - holds original hash  
   - contains PoLIFE / PoLABOR / PoHW records  

2. **Public Protocol Repo**  
   - holds documentation  
   - does *not* hold raw data  
   - holds schemas  
   - holds proof templates  
   - holds registry  

This separation is mandatory.

---

# 4. Daily Workflow (Simple Version)

Here is the minimum version of the DGCP workflow:

### Step 1 — Capture Real Life
Take photos/videos of:
- morning conditions  
- farm environment  
- labor actions  
- events  
raw/YYYY-MM-DD/
polife/
polabor/
pohw/

### Step 3 — Compute SHA-256
Hash must match:
- raw file  
- IPFS file (if uploaded later)

### Step 4 — (Optional) Upload to IPFS
Write down:
- CID  
- gateway links  
- timestamp  

### Step 5 — Create a Proof Entry
Create proof-XXX file in your public repo:
- link IPFS  
- include hash  
- include context  
- follow template  

### Step 6 — Registry Update
Append entry into `registry.md`.

Consistency = protocol compliance.

---

# 5. Data Integrity Requirements

DGCP requires:

1. **No rewriting**  
2. **No modifying raw files**  
3. **No renaming original images**  
4. **No “cleaning” camera metadata**  
5. **No synthetic or AI-shaped data**  
6. **No loss of timestamps**  
7. **No compression artifacts**  

Once a file is captured → it becomes part of history.

---

# 6. Human Context Implementation

Every proof entry must include a short human context line:
- why the moment mattered  
- what happened  
- emotional truth  
- real-life meaning  

DGCP is the first protocol to embed this requirement.

---

# 7. IPFS / NFT Optional Layer

You may:
- publish selected evidence to IPFS  
- mint NFT as a timestamp anchor  

But:
- IPFS is permanent  
- NFT is optional  
- neither replace the private repo  

The private repo is always the origin of truth.

---

# 8. Governance for Implementers

Anyone implementing DGCP must:

- respect the MMFARM-POL-2025 License  
- preserve attribution:  
  **“DGCP Protocol by MaMeeFarm (P’Tōh)”**  
- avoid commercial use without permission  
- maintain append-only integrity  
- protect raw human-origin truth  

DGCP is a human-first protocol, not a data mining tool.

---

# 9. Example Folder Structure (Suggested)

private-repo/
raw/
2025-01-12/
IMG_0012.JPG
polife/
polabor/
pohw/
hashes/
ipfs-log/
notes/

public-repo/
proof/
proof-001.md
proof-002.md
registry.md
schema/
protocol/
layers/
governance/
---

Simple, but powerful.

---

# 10. Common Mistakes to Avoid

- mixing raw data into public repo  
- editing a previous proof file  
- using cloud compression (LINE, Messenger, etc.)  
- renaming raw images after capture  
- allowing others to access private repo  
- losing timestamps  
- writing context “after the fact”  

DGCP = consistency + integrity.

---

# Closing Thoughts

DGCP is not only a protocol.  
It is a new class of human-origin evidence.

Implementation is not about perfection.  
It is about honesty, discipline, and respecting real work.

DGCP exists so ordinary people  
can hold their truth in a world moving faster than them.

---

**Maintainer:**  
P’Toh — MaMeeFarm™  
Lampang, Thailand

### Step 2 — Store Raw Files
Move files to private repo:
