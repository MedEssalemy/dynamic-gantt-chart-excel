# 📊 Dynamic Gantt Chart Template – Advanced Excel Planning Engine

I built this Excel Gantt Chart for structured project environments where basic templates are not enough. This is not a “colored bar” spreadsheet—it is a **fully formula-driven scheduling engine** designed to handle real-world complexity.

## 🚀 What Makes This Different?
Most Excel Gantt charts support only a single start date and duration with no baseline or change tracking. This engine supports:

* **✔ Multi-date tasks** & **Multi-duration logic**
* **✔ Automatic rescheduling** & **Extension detection**
* **✔ Baseline preservation**
* **✔ Milestone automation**
* **✔ Dynamic timeline engine**

> **Note:** No VBA required. 100% formula-based using modern Excel dynamic arrays.

---

## 📌 Multi-Date & Multi-Duration Support
You can define multiple start dates and durations using semicolon separation. Dates must follow **ISO format (YYYY-MM-DD)**.

**Example 1:**
* **Start Date:** `2026-01-07; 2026-01-20`
* **Duration:** `5`
* *Result:* Two separate phases, both lasting 5 days.

**Example 2:**
* **Start Date:** `2026-01-07; 2026-01-20`
* **Duration:** `5; 4`
* *Result:* Phase 1 (5 days) and Phase 2 (4 days).

This allows for split execution phases, multi-wave implementation, and structured work packages.

---

## 🔄 Rescheduling Logic
* **Rescheduling:** If “Revised Start” is filled, the task becomes rescheduled, but the original baseline remains visible.
* **Extension Detection:** If `Revised Duration > Original Duration`, the extended portion is automatically highlighted, making scope changes visible immediately.
* **Milestone Automation:** Set `Duration = 0` and the system automatically displays a milestone marker on the timeline.

---

## 📊 Timeline Visual Logic
Everything is calculation-driven and follows this visual key:

| Indicator | Meaning |
| :--- | :--- |
| **Light Green** | Planned duration |
| **Dark Green** | Rescheduled duration |
| **Red** | Extension |
| **Gray Hashed** | Original baseline |
| **Dot** | Milestone |

---

## ⚙️ Technical Architecture
Built using modern Excel functions for high performance:
* **Dynamic Arrays** & **LET()** structured formulas
* **TEXTSPLIT()** for multi-date parsing
* **Named functions:** `ParseDates()`, `GetEndDates()`

The timeline recalculates dynamically based on the project start date.

---

## 🎯 Designed For
* Industrial programs & Automotive modernization
* IT deployments & ERP implementation
* Structured multi-phase projects

## 💡 Why I Built This
In structured environments, project tracking needs traceability and change visibility. Excel is often underestimated; with modern functions, it becomes a powerful project engine. 

If you are working on complex Excel systems or structured planning environments—I’d be happy to exchange ideas.

---
`#Excel` `#ProjectManagement` `#Automation` `#GanttChart` `#BusinessTools` `#Planning`
