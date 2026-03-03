# Lab: Calculating TCO for a Multi-Agent Swarm

## 🎯 Objective
In this lab, you will act as the "AI Financial Analyst" and build a 1-year **Total Cost of Ownership (TCO)** model for a multi-agent system.

## 🏢 Scenario Context
**Company:** "GlobalDispatch Inc."
**Project:** "Swarm-1" - 5 specialized agents (Customs, Route, Carrier, Weather, Pricing) orchestrating 1,000 global shipments per day.
**The Challenge:** The CEO is worried that the "per-token" costs of using a frontier model (GPT-4) will erode the profit margins of the shipping business.

---

## 🛠️ The Cost Drivers (Mock Data)
| Component | Annual Cost (Est) |
| :--- | :--- |
| **Model APIs (Tokens)** | $0.05 per shipment (Avg) x 1,000 shipments/day x 365 days. |
| **Vector DB (Storage)** | $500 / month. |
| **Cloud Hosting (Azure/AWS)** | $1,200 / month. |
| **Maintenance & Monitoring** | $4,000 / month (1 part-time engineer). |
| **Human-in-the-Loop (Audit)** | $3,000 / month (Expert review of 5% of cases). |

---

## 📝 Exercise 1: The Raw TCO Calculation
Calculate the Total Annual Cost for "Swarm-1" based on the figures above.

---

## 📊 Exercise 2: ROI Break-Even Analysis
If each autonomously resolved shipment saves the company **$0.25** in labor and penalties:
*   **Question:** What is the total annual "Gross Value" created?
*   **Question:** Is the project profitable in Year 1?

---

## ✅ Deliverable
Draft a 1-page "Financial Impact Report." 
*   **Section 1:** Total Annual TCO.
*   **Section 2:** Net Profit / Loss.
*   **Section 3:** Cost Optimization Strategy (e.g., "Switching to a cheaper SLM for the Triage Agent could save 20% on token costs").
