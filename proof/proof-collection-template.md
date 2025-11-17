# DGCP Proof Collection – {PROOF_ID}

**Location:** MaMeeFarm™ – Lampang, Thailand  
**Protocol Layer:** PoLIFE / PoLABOR / PoHW / DGCP  
**Proof ID:** `{PROOF_ID}`  
**DGCP Version:** `1.0.0`  

---

## 1. Summary

- **Date range:** {DATE_RANGE}  
- **Scope:** {SCOPE_DESCRIPTION}  
- **Context:** {SHORT_CONTEXT}  
- **Created by:** P’Tōh — MaMeeFarm™  

This file does not store raw data.  
It points to evidence that already exists in other systems.

---

## 2. Linked Evidence (Off-Chain)

### 2.1 GitHub (Primary Evidence)
Repository: `MaMeeFarm-Data`  
Path: `{GITHUB_PATH}`  
Commit hash: `{GITHUB_COMMIT_HASH}`  

This is the first public checkpoint of the record.

---

### 2.2 IPFS (Permanent Storage)
- IPFS CID: `{IPFS_CID}`  
- Gateway example: `https://ipfs.io/ipfs/{IPFS_CID}`  

The CID must match the SHA-256 hash of the original content.

---

## 3. Linked Evidence (On-Chain / NFT)

*(Optional — only if minted)*

- Network: `{CHAIN_NAME}` (e.g. Polygon)  
- Contract address: `{CONTRACT_ADDRESS}`  
- Token ID: `{TOKEN_ID}`  
- Block / transaction reference: `{TX_HASH_OR_LINK}`  
- Marketplace link (optional): `{OPENSEA_OR_MARKET_URL}`  

On-chain tokens are pointers.  
They do not replace the original evidence.

---

## 4. Related DGCP Units

List the related protocol-level records.

- PoLIFE events:  
  - `schema/polife-event.schema.json` → see data in MaMeeFarm-Data  
- PoLABOR tasks:  
  - `schema/polabor-task.schema.json` → see data in MaMeeFarm-Data  
- PoHW units:  
  - `schema/pohw-unit.schema.json` → combined human work proofs  

Each linked record must remain immutable.

---

## 5. Integrity Check

All evidence in this collection must be verifiable.

- Primary hash (SHA-256): `{PRIMARY_HASH}`  
- Optional additional hashes:  
  - `{HASH_1_DESCRIPTION}` – `{HASH_1_VALUE}`  
  - `{HASH_2_DESCRIPTION}` – `{HASH_2_VALUE}`  

Verification steps:
1. Fetch the file from GitHub or IPFS.  
2. Compute SHA-256 on the raw content.  
3. Compare with `PRIMARY_HASH`.  
4. If it does not match, the record is not valid DGCP evidence.

---

## 6. Human Context (Non-Editable)

This section provides short human context for the proof.

- What happened: `{HUMAN_EVENT_SUMMARY}`  
- Who worked: `P’Toh and MaMeeFarm family`  
- Why it matters: `{WHY_IT_MATTERS}`  

This section must be written once and never rewritten.  
If something needs to be added, create a new proof collection  
and link back to this one.

---

## 7. Governance

This proof collection is covered by:

- `license.md` — MMFARM-POL-2025 License  
- `governance/governance-protocol.md` — IP Governance rules  

All rights belong to **P’Toh — MaMeeFarm™**.  
Historical truth must remain as it was.
