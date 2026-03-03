# Lab: Building an Agent-Ready Knowledge Base

## 🎯 Objective
In this lab, you will learn how to structure unstructured documents (PDFs, Word docs, Wiki pages) to optimize them for **Retrieval-Augmented Generation (RAG)**.

## 🛠️ Scenario Context
You have been given 50 different PDF files containing "Shipping Policies" for various countries. Some are 1 page, some are 40 pages. 

**The Goal:** Prepare these documents so a "Shipping Expert Agent" can answer questions with 99% accuracy.

---

## 📝 Exercise 1: Content Chunking Strategy
If you pass a 40-page PDF into an LLM context window at once, it might "get lost in the middle" or exceed the token limit.
*   **Question:** Would you recommend chunking by *Character Count* (e.g., every 500 characters) or *Semantic Heading* (e.g., every section title)? 
*   **Rationale:** Explain why your chosen method is better for a BA to manage.

---

## 📊 Exercise 2: Metadata Tagging
Adding "Tags" to your documents helps the Vector Database find the right info faster.
**Task:** For a document titled "Customs-Regulations-Italy-2024.pdf", suggest 5 metadata tags that would help an AI agent route the query correctly.

*Example Tags:* `Region: EMEA`, `DocumentType: Regulatory`, `EffectiveDate: 2024-01-01`...

---

## ✅ Deliverable
Draft a "Knowledge Base Governance Policy" (1 page). 
*   How often should docs be updated? 
*   Who is responsible for the "Golden Source" of truth? 
*   How do we handle "Retired" documents so the AI doesn't give outdated advice?
