# Lab: The Data Readiness Audit (DRA)

## 🎯 Objective
As an AI Business Analyst, you must evaluate whether a legacy dataset is "ready" to power a high-stakes AI agent. In this lab, you will perform a mock audit of a legacy Customer Relationship Management (CRM) database to identify risks and blockers for a RAG-based integration.

## 🏢 Scenario Context
**Company:** "LegacyRetail Inc."
**Project:** Project "Insight" - An AI agent designed to summarize customer history for sales reps before a call.
**The Challenge:** The data is stored in an 18-year-old SQL database with inconsistent formatting, missing fields, and no clear data lineage.

---

## 🛠️ The Data Sample (Mock Audit Observations)
| Field Name | Observation |
| :--- | :--- |
| `LastPurchaseDate` | 35% of records are empty (NULL). |
| `CustomerNotes` | Free-text field. Contains everything from product feedback to internal jargon like "VIP-99" and "DO-NOT-CALL." |
| `PurchaseHistory` | Stored as a giant JSON blob that hasn't been validated in 4 years. |
| `PII_Flag` | There is no indicator of which fields contain sensitive PII (Personally Identifiable Information). |

---

## 📝 Exercise 1: Identifying "Data Friction"
Based on the observations above, identify the 3 biggest risks this data poses to an AI agent. 

*Example:* "The inconsistent `CustomerNotes` field might lead the agent to hallucinate customer sentiment or accidentally repeat internal-only jargon to a customer."

---

## 📊 Exercise 2: The Readiness Scorecard
Rate the data from 1 to 5 (1 = Not Ready, 5 = Production Ready) for the following criteria:
1.  **Completeness:** (e.g., Are there too many NULLs?)
2.  **Cleanliness:** (e.g., Is the text normalized?)
3.  **Accessibility:** (e.g., Can an API easily fetch the JSON blobs?)
4.  **Governance:** (e.g., Is PII identified and protected?)

---

## ✅ Deliverable
Draft a 2-paragraph "Data Remediation Plan" for the Data Engineering team. 
*   What needs to be cleaned first? 
*   Do we need to synthesize data to fill the gaps? 
*   What guardrails must be built at the database level before the LLM can access this info?
