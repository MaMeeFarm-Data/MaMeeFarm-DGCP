# DGCP™ System Behavior — Sensor Anomaly Behavior
*Version 1.0.0 — MMFARM-POL-2025 Licensed*

This document describes how DGCP™ behaves when sensor data (temperature, humidity, etc.) appears abnormal, inconsistent, or unreliable.

---

## 1. Anomaly ≠ Error by Default

Unusual sensor values may reflect:

- real extreme conditions  
- device malfunction  
- human misuse  

DGCP must not assume “device error” automatically.

---

## 2. Parallel Truth Principle

When a sensor anomaly is detected, DGCP should preserve:

- raw sensor value (as recorded)  
- human perception (if provided)  
- contextual notes (cold, hot, windy, storm, etc.)

Parallel truths are allowed.

---

## 3. No Automatic Smoothing

DGCP must not:

- smooth spikes  
- average out extremes  
- “correct” values to fit expectations  

Spikes might be the most important part of the data.

---

## 4. Flagging Behavior

If values are suspicious (e.g. impossible range):

- DGCP may flag them as “anomalous”  
- add a short note: “outside normal device range”  
- keep original value intact.

Flagging is annotation, not modification.

---

## 5. Cross-Checking Behavior

When possible, DGCP may:

- cross-check with adjacent readings  
- compare with time-near events (photos of frost, humans in coats, etc.)  
- log whether anomaly seems plausible given context.

But cross-checking must never overwrite the original reading.

---

## 6. Human Override on Sensors

If the human states:

- “device was broken that day”  
- “this reading is clearly wrong”  

DGCP may:

- mark the reading as “human-confirmed invalid”  
- keep the raw reading  
- add a human-adjusted narrative value **as a separate field**.

Raw data stays; human judgment is layered on top.

---

## 7. Behavior Under Missing Calibration

If devices are low-cost or poorly calibrated:

- DGCP acknowledges limitations in metadata  
- emphasizes relative patterns over absolute precision  

“Cheap sensor truth” is still valuable truth.

---

## 8. No Retroactive Recalculation

If a sensor is later calibrated:

- DGCP may add new calibration notes  
- may interpret past data differently at analysis time  
- but must not rewrite historical raw values.

Past readings belong to their own technological era.

---

## 9. Anomaly Logging

For anomalies, DGCP should log:

- value(s) observed  
- time and location  
- anomaly type (extreme, inconsistent, impossible)  
- human comments (if any)

This supports later scientific and governance work.

---

## 10. Alignment with DGCP Philosophy

Sensor anomaly behavior must:

- protect raw reality  
- highlight uncertainty instead of hiding it  
- empower later analysis without fabricating data  

Low-cost, imperfect sensors at MaMeeFarm™  
are part of the story — not a flaw to erase.

---

**License**  
This file is licensed under MMFARM-POL-2025 + CC BY-NC 4.0  
Human-first, Reality-aligned, DGCP-governed.
