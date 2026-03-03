# Lab: Bias Audit of a Resume-Scanning Agent

## 🎯 Objective
As an AI-Expert BA, you are responsible for the **Governance** of autonomous systems. In this lab, you will perform a "Bias Audit" on a mock dataset used to train an HR Resume-Scanning Agent to identify potential algorithmic discrimination.

## 🏢 Scenario Context
**Company:** "FutureHire AI."
**Problem:** The recruiting team noticed that the AI is disproportionately ranking candidates from Ivy League schools higher, even if their experience is identical to candidates from state universities.
**The Challenge:** You must prove *where* the bias is coming from—the training data, the prompt, or the model itself—and propose a mitigation strategy.

---

## 🛠️ The Audit Data (Mock Analysis)
**Training Data History:** 10,000 successful past hires from 2010–2024.
*   **Fact 1:** 85% of past "Successful Hires" came from Top 10 Ranked Universities.
*   **Fact 2:** 70% of those hires were male.
*   **Fact 3:** The model was told to "replicate the profile of our most successful historical employees."

---

## 📝 Exercise 1: Identifying the "Historical Bias"
Why is the model ranking Ivy League candidates higher? 
*   **Question:** Is this a "Model Error" or a "Data Mirroring" error?
*   **Rationale:** Explain how the model's goal ("replicate our past success") is conflicting with modern Diversity & Inclusion (DEI) goals.

---

## 📊 Exercise 2: Mitigation Strategy
Suggest 3 specific "Guardrails" you would put in place to ensure the AI focuses on **Skills** rather than **Prestige**.

*Example Guardrail:* "PII Scrubbing: Before the resume hits the LLM, a pre-processor agent must strip the name of the University and the Candidate's Name to prevent gender and prestige bias."

---

## ✅ Deliverable
Draft a 1-page "AI Ethics Audit Report" for the VP of HR. 
*   What is the root cause of the bias?
*   What is the risk of *not* fixing it (e.g., Legal / Regulatory)?
*   What is the "Human-in-the-Loop" (HITL) step you recommend for the final hiring decision?
