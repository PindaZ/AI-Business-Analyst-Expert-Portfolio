# Knowledge Check: Phase 2 Data Strategy & Readiness

Test your proficiency in modern AI data architecture and readiness.

---

## Scenario 1: The RAG Context Window Limit
**Context:** Your "Global Support Agent" needs to access a 2,000-page "Master Manual" to answer questions. 
**Problem:** The LLM's context window is only 128k tokens (roughly 100 pages). 
**Question:** What architecture would you propose to solve this?
- A) Fine-tune a model on the entire 2,000-page manual.
- B) Use a Vector Database to retrieve only the relevant chunks (RAG).
- C) Ask the user to upload only the relevant chapter of the manual.
- D) Manually rewrite the manual to be shorter.

**Answer & Rationale:** **B (RAG)**. 
Fine-tuning is expensive, hard to update, and might not "remember" specific facts as accurately as a retrieval-based system. RAG is the enterprise standard for this use case.

---

## Scenario 2: The Data Moat
**Context:** A medical startup is using publicly available research papers to build a "Diagnostic Assistant." A competitor uses the same papers but adds 500,000 proprietary, anonymized patient outcomes from a local hospital network.
**Question:** Which company has a "Data Moat"?
- A) Both (The research papers are valuable).
- B) Neither (Public models like GPT-4 already know the papers).
- C) The competitor with the proprietary hospital data.
- D) The startup with the public research papers.

**Answer & Rationale:** **C (Competitor)**. 
A Data Moat is built on **proprietary, non-commodity data**. Public research is available to everyone, including frontier model developers, and provides zero competitive advantage.

---

## Scenario 3: Real-Time Integration
**Context:** An "E-commerce Inventory Agent" is telling customers that a product is "In Stock," but when they try to pay, it's actually sold out. 
**Problem:** The agent's knowledge base is updated once every 24 hours.
**Question:** What is the technical "Readiness" blocker here?
- A) Model Intelligence (The LLM is hallucinating).
- B) Data Freshness/Latency (The agent lacks real-time API access).
- C) Token Cost (Updating more often is too expensive).
- D) Prompt Engineering (The system prompt needs more clarity).

**Answer & Rationale:** **B (Freshness/Latency)**. 
The agent needs a "Tool" or "API" that can query the live inventory database at the moment the customer asks, rather than relying on a static, outdated knowledge base.

---

## Final Score Logic:
- **3/3:** Data Architect. You understand the "Readiness" challenges of 2026.
- **0-2/3:** Practitioner. Revisit the **RAG Data Strategy** and **Real-Time Data Integration** modules.
