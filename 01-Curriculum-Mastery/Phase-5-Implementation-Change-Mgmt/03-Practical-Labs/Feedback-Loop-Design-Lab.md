# Lab: Designing a Continuous Feedback Loop

## 🎯 Objective
In this lab, you will design the **Human-AI Interface** that allows subject matter experts (SMEs) to correct and "train" the AI system without writing a single line of code.

## 🛠️ Scenario Context
**Company:** "LegalDocs AI."
**Problem:** The AI is summarizing legal contracts, but it consistently gets the "Force Majeure" clause wrong for European contracts. 
**The Goal:** Build a feedback loop so a lawyer can correct the error and ensured the AI learns from it.

---

## 📝 Exercise 1: The "Correction" UI
Sketch (or describe) the UI for the feedback loop. 
*   **Question:** Should it be a simple "Thumbs Up/Down" button, or a "Suggest Edit" field? 
*   **Rationale:** Why is the "Suggest Edit" field more valuable for the AI's long-term accuracy?

---

## 📊 Exercise 2: The "Reward" Mechanism (RLHF)
Once a lawyer corrects the AI, what happens to that correction? 
1.  Is it ignored?
2.  Is it added to the RAG database for future reference?
3.  Is it used to "Reward" the model during future fine-tuning?

**Task:** Propose a workflow (1 paragraph) that ensures the AI doesn't make the same mistake twice.

---

## ✅ Deliverable
Draft a "Human-in-the-Loop Governance Policy." 
*   Who is authorized to "Correct" the AI?
*   How do we ensure the corrections themselves aren't biased?
*   How do we measure the "Improvement Rate" over time?
