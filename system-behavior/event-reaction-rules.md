# DGCP™ System Behavior — Event Reaction Rules
*Version 1.0.0 — MMFARM-POL-2025 Licensed*

This document defines how the DGCP™ protocol reacts when a real-world event is captured by a human worker.

DGCP does not create events.  
DGCP only **reacts** to reality.

---

## 1. Event-First, System-Second

1. A real-world event happens.  
2. A human decides to capture it (photo, video, text, measurement).  
3. DGCP receives the capture and reacts according to these rules.

The protocol never initiates, schedules, or simulates events.

---

## 2. Minimal Reaction Principle

DGCP reacts with the **minimum necessary behavior**:

- store the proof  
- register the event  
- link to the correct day / context / chain  
- document its own behavior in logs  

If a reaction is not necessary to preserve truth, it must not occur.

---

## 3. One Event → One Primary Reaction

For every event:
- exactly one **primary reaction** is allowed  
- secondary reactions must be traceable back to the primary one  

No duplicate “first reactions” are allowed.

---

## 4. Respect for Human Timing

If the worker:
- captures late  
- uploads late  
- processes late  

DGCP must preserve the worker’s timing as metadata  
and must not pretend that the event was processed earlier.

---

## 5. No Forced Categorization

If an event:
- does not fit predefined categories  
- is messy or mixed (farm + personal + weather)  

DGCP must still accept it without forcing a simplified label.

Unclear events are still valid events.

---

## 6. Reaction to Composite Events

If one capture contains multiple realities (e.g. duck, dog, weather, human emotion):

- DGCP registers a **single event with multiple facets**,  
  not multiple fake events.  
- Each facet can be tagged in metadata, but the event remains one.

---

## 7. Human-Corrected Reaction

If the worker later clarifies:
- what actually happened  
- what the event means  
- why it was important  

DGCP may add a **human explanation layer**,  
but may not rewrite or replace the original reaction.

---

## 8. No Automated Escalation

DGCP must not:
- escalate events by itself  
- classify them as “critical”, “urgent”, or “alert-level”  
without explicit human-defined rules in a higher governance layer.

---

## 9. Reaction Logging

Every reaction should be:
- logged in a simple, human-readable form  
- linked to the original proof ID  
- clearly explainable in a single sentence

If the reaction cannot be explained in plain language,  
the reaction is invalid.

---

## 10. Alignment with Core Rules

All event reactions must comply with:

- Once-Only Principle  
- Non-Interference  
- Zero Optimization  
- Fail-Silent Behavior  

If a conflict appears, **Core Rules override Event Rules.**

---

**License**  
This file is licensed under MMFARM-POL-2025 + CC BY-NC 4.0  
Human-first, Reality-aligned, DGCP-governed.
