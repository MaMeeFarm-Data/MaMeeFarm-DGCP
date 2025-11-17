# DGCP Versioning Model  
Version 1.0 (2025)

This document explains how DGCP evolves over time without breaking  
historical truth. All updates must follow the DGCP versioning model.

DGCP uses **SPV — Semantic Protocol Versioning**  
with three components:

MAJOR.MINOR.PATCH

Example:
1.0.0
1.1.0
2.0.0

---

## 1. MAJOR Version (Breaking Structure Changes)

A MAJOR update is applied when:
- schema structure changes  
- fields are added or removed  
- a layer definition changes  
- data flow or verification rules are updated  
- governance rules change meaning  

MAJOR updates create a **new protocol era**.

Past data remains under the previous major version and is never altered.

Examples:
- 1.x.x → 2.0.0  
- 2.x.x → 3.0.0  

MAJOR updates require:
- whitepaper update  
- governance update  
- full changelog entry  
- schema version bump  

---

## 2. MINOR Version (New Features, No Breaking Change)

A MINOR update is applied when:
- new fields are added (optional)  
- new examples are added  
- clarifications are made  
- non-breaking improvements occur  
- new documentation is added  

Examples:
- 1.0.0 → 1.1.0  
- 1.1.0 → 1.2.0  

MINOR updates never break existing data.

---

## 3. PATCH Version (Small Fixes)

A PATCH update is for:
- typos  
- formatting corrections  
- small comments added  
- non-structural clarifications  
- example corrections that do not affect meaning  

Examples:
- 1.0.0 → 1.0.1  
- 1.0.1 → 1.0.2  

PATCH changes do not affect protocol behavior.

---

## 4. Versioning Rules for Schemas

Each schema file includes:
- `"version": "1.0.0"`  
inside the JSON definition (added later).

Rules:
- MAJOR → change schema file name  
- MINOR → keep name, update version  
- PATCH → update version only  

No schema may remove required fields in a MINOR or PATCH version.

---

## 5. Versioning Rules for Proof Units

PoLIFE, PoLABOR, PoHW units remain under their creation version forever.

Example:
If a PoHW unit was created during DGCP **v1.0**,  
it is never upgraded to **v1.1** or **v2.0**.

Proof units are immutable.

---

## 6. Versioning Documentation

Each version bump requires:
- entry in `changelog.md`  
- schema version update  
- no rewriting of past records  

DGCP evolves  
but history stays still.

---

## 7. Current Protocol Version

**DGCP Version: 1.0.0 (Initial Release)**  
Released: 2025  
Maintainer: P’Toh — MaMeeFarm™

