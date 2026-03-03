# Knowledge Check: Phase 4 Conceptual AI Architecture

Test your ability to design scalable, cost-effective, and robust Agentic systems.

---

## Scenario 1: Router Architecture
**Context:** Your customer asks: *"Where is my order?"* in Spanish.
**Problem:** Your "Shipping Agent" only knows English policies.
**Question:** What architecture would solve this?
- A) A single model trained on all languages.
- B) A "Router Agent" that detects the language and routes to a "Translator Agent" or a language-specific RAG system.
- C) Ask the user to repeat the question in English.
- D) A manual human translator.

**Answer & Rationale:** **B (Router Agent)**. 
A router detects intent or language and sends the query to a specialized model, reducing the context window and cost compared to a single "do-it-all" model.

---

## Scenario 2: SLMs vs. LLMs
**Context:** Your "Summarization Agent" needs to run on an iPhone without internet access.
**Problem:** A 70B parameter LLM is 140GB and won't fit on the device.
**Question:** What is the most likely solution?
- A) Use a cloud-based GPT-4 API.
- B) Use a Small Language Model (SLM) like Phi-3 or Gemma, optimized for mobile (edge) performance.
- C) Delete all other apps on the iPhone to make room.
- D) Tell the user the summary isn't available offline.

**Answer & Rationale:** **B (SLM)**. 
SLMs are designed for "Edge AI," where local execution, low latency, and low memory are prioritized over broad general intelligence.

---

## Scenario 3: Agentic Memory
**Context:** A user asks: *"What did I say yesterday about the return?"* 
**Problem:** The AI resets its context after every session.
**Question:** What architecture is missing here?
- A) Short-term Memory (Context window).
- B) Long-term Memory (Vector database or user profile storage).
- C) Model Fine-tuning.
- D) Recursive Logic.

**Answer & Rationale:** **B (Long-term Memory)**. 
To recall information across sessions, the AI needs to store the interaction in a user-specific "Memory" database and retrieve it when the user returns.

---

## Final Score Logic:
- **3/3:** System Architect. You understand the "Modular AI" of 2026.
- **0-2/3:** Practitioner. Revisit the **Router Architecture** and **SLMs vs. LLMs** modules.
