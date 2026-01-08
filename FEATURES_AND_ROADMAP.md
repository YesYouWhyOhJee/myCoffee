# ☕ myCoffee — Features & Roadmap

**Your personal coffee journal**

This document defines the **functional requirements**, **non-functional requirements**, and **development roadmap** for the myCoffee web application.

It is intended to guide development decisions, prevent scope creep, and keep the product aligned with its core purpose over time.

---

## 1. Functional Requirements (FR)

### FR-1: Guided Brewing
- The system shall guide the user through a coffee brew using predefined steps.
- Each brew step shall include:
  - Target time (seconds)
  - Water amount (grams)
  - Instructional text
- The system shall display a timer that indicates progress through the brew.

---

### FR-2: Recipe Representation
- The system shall represent a coffee recipe with the following properties:
  - Recipe name
  - Brew method (e.g., pour-over)
  - Coffee dose (grams)
  - Total water dose (grams)
  - Grind size descriptor
  - Water temperature (°C)
  - Ordered list of brew steps

---

### FR-3: Brew Session Tracking
- The system shall record a brew session upon completion.
- A brew session shall include:
  - Recipe used
  - Brew start time
  - Actual total brew duration
  - Optional user notes
  - Optional user rating

---

### FR-4: Brew History
- The system shall store completed brew sessions locally in the user's browser.
- The user shall be able to view a chronological list of past brew sessions.

---

## 2. Non-Functional Requirements (NFR)

### NFR-1: Performance
- Timer updates shall be accurate to within ±1 second.

---
