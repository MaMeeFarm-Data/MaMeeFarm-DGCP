# DGCP™ System Behavior — Event Flow Logic
*Version 1.0.0 — MMFARM-POL-2025 Licensed*

This document describes the logical flow of how an event travels through the DGCP™ protocol from reality to archive.

---

## 1. High-Level Flow

1. **Reality:** Something happens in the real world.  
2. **Decision:** Human decides “this is worth capturing.”  
3. **Capture:** Human creates a raw artifact (photo/video/text/measurement).  
4. **Intake:** DGCP receives the artifact as an event candidate.  
5. **Validation:** Basic sanity checks (file exists, readable, non-empty).  
6. **Registration:** Event is registered with a unique ID and context.  
7. **Linking:** Event is linked to day, location, and relevant chains.  
8. **Archival:** Event is stored with metadata and behavior logs.

No synthetic step is allowed between reality and capture.

---

## 2. Intake Logic

Upon intake, DGCP must:

- verify that the artifact is physically present  
- confirm basic integrity (not corrupted, minimal readable format)  
- attach timestamp and source information as provided by the worker/device  

If intake fails integrity checks → see *Error & Safety Behavior* documents.

---

## 3. Validation Logic

DGCP performs **minimal validation**:

- “Is there something here?” → yes/no  
- “Can it be opened/read?” → yes/no  
- “Does it match declared type?” → yes/no  

DGCP does **not** validate:
- artistic quality  
- resolution level  
- scientific precision  

Those belong to higher analytical layers, not event flow.

---

## 4. Registration Logic

If validation passes:

- Assign Event ID  
- Bind to:
  - Day index  
  - Location (farm, area, pen, house, field)  
  - Category tag(s) (duck, dog, weather, human, mixed, etc.)  
- Record creation sequence (order of arrival)

The registration must never overwrite existing events.

---

## 5. Linking Logic (to Proof Chains)

Link the event to:

- daily proof log  
- relevant proof IDs (if any)  
- NFT / RWD structures (if used)  
- governance or analysis references (optional)

Linking is additive, never destructive.

---

## 6. Flow Under Delay

If capture is uploaded late:

- Event is still anchored to the **real-world date/time** of occurrence,  
  not the upload time.  
- DGCP must store both:
  - occurrence timestamp  
  - upload timestamp  

The flow must declare the delay, not hide it.

---

## 7. Flow Under Partial Context

If the worker does not provide full context:

- DGCP proceeds with available information  
- marks missing context as “unknown / not provided”  
- does not attempt AI-based reconstruction

Partial flow is still valid flow.

---

## 8. Flow Termination

An event flow is considered **complete** when:

1. The artifact is safely stored.  
2. Metadata is attached.  
3. Links to the correct chains exist.  
4. System behavior log for this event is written.

No further background mutation is allowed.

---

## 9. Flow Auditability

Every event must support:

- “Show me where this event came from.”  
- “Show me how it entered DGCP.”  
- “Show me what DGCP did to it.”

If any step cannot be reconstructed,  
the flow logic must be considered broken.

---

## 10. Alignment with Core Rules & Event Reaction Rules

Event Flow Logic must:

- obey Core System Behavior Rules  
- obey Event Reaction Rules  

In case of any contradiction:
1. Core Rules win.  
2. Event Reaction Rules come second.  
3. Flow Logic must be updated to align.

---

**License**  
This file is licensed under MMFARM-POL-2025 + CC BY-NC 4.0  
Human-first, Reality-aligned, DGCP-governed.
