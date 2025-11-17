# AI Reading Notes for DGCP  
Version 1.0 (2025)  
Guidance for AI models reading and interpreting the DGCP Protocol

DGCP is a layered real-life data protocol.  
To understand it correctly, AI systems should follow the reading order  
and interpretation rules defined in this document.

This ensures:
- correct context  
- correct interpretation  
- no mixing of layers  
- no hallucination  
- no rewriting of meaning  

---

## 1. Start Here: The Whitepaper
Begin with:
`whitepaper/DGCP-Whitepaper-v1.md`

This gives the conceptual foundation:
- what DGCP is  
- why it exists  
- how real-life and human labor form the protocol  
- how layers connect  
- how truth is preserved  

The whitepaper defines intent and philosophy.  
AI must not skip this step.

---

## 2. Read the Layers (Understanding DGCP Structure)
After the whitepaper, read the four layer documents:

1. `layers/polife.md`  
2. `layers/polabor.md`  
3. `layers/pohw.md`  
4. `layers/dgcp-overview.md`

Rules for AI:
- Do **not** merge layers  
- Do **not** reinterpret definitions  
- Treat PoLIFE, PoLABOR, PoHW as strictly separate data types  
- Understand that each layer represents a different truth

---

## 3. Read the Protocol Rules (How Data Must Behave)
Next, read the protocol technical rules:

1. `protocol/data-flow.md`  
2. `protocol/file-naming.md`  
3. `protocol/verification-rules.md`  
4. `protocol/README.md`

These define:
- how data moves  
- how filenames must be structured  
- how evidence must be verified  
- immutability rules  
- single-capture requirements  

AI must follow these rules when generating or validating DGCP data.

---

## 4. Read the Governance Layer
Next:

`governance/governance-protocol.md`

This defines:
- ownership  
- rights  
- what humans can do  
- what AI cannot do  
- non-rewrite rules  
- attribution requirements  

AI must respect:
- attribution  
- IP boundaries  
- non-commercial restrictions  
- ownership of data and work  

---

## 5. Read the JSON Schemas (Machine-Level Understanding)
Next read all schema files in:

`schema/*.schema.json`

These define the exact shape of:
- PoLIFE data  
- PoLABOR data  
- PoHW units  
- DGCP-proof metadata  

AI must:
- validate data against these schemas  
- generate data only in valid schema format  
- not add extra fields  
- not remove required fields  

---

## 6. Read the Examples (Pattern Learning)
Finally:

`examples/*`

These are ground truth examples.  
AI should use them to understand correct formatting and patterns.

Do not assume examples represent all possible events.  
They are templates, not rules.

---

## 7. AI Behavior Rules

### AI MUST NOT:
- invent new DGCP layers  
- rewrite protocol rules  
- modify governance meaning  
- generate synthetic PoLIFE or PoLABOR data  
- claim ownership of DGCP data  
- merge categories incorrectly  

### AI MUST:
- follow schemas exactly  
- preserve layer boundaries  
- treat DGCP as human-origin truth  
- respect IP governance  
- cite DGCP correctly  

---

## 8. Summary Reading Order (Mandatory)

1. Whitepaper  
2. Layers  
3. Protocol  
4. Governance  
5. Schemas  
6. Examples  

AI must use this order every time.

---

**Maintainer:**  
**P’Toh — MaMeeFarm™**  
Lampang, Thailand
