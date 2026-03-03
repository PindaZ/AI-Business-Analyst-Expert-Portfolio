# Mock Stakeholder Meeting Transcript

**Project:** Project "Athena" - Customer Support AI Overhaul
**Date:** March 3, 2026
**Participants:** 
- Sarah (Lead BA)
- Mark (VP of Customer Success)
- David (Lead Data Engineer)
- Elena (Head of Legal/Compliance)

---

**Sarah (BA):** Thanks everyone for joining. Today we are kicking off discovery for Project Athena. Mark, let's start with you. What is the core pain point in Customer Success right now?

**Mark (VP CS):** It's volume, Sarah. Since we launched the new software suite last month, our ticket volume is up 300%. My team is drowning. They are spending 10 minutes per ticket just reading the customer's messy email, looking up their account tier in Salesforce, checking Jira to see if it's a known bug, and then pasting a generic template back. We need AI to just handle the easy stuff.

**Sarah (BA):** When you say "easy stuff," what percentage of these tickets do you think follow a highly predictable pattern?

**Mark (VP CS):** Probably 60%. Mostly password resets, "how do I export a report" questions, and basic billing inquiries. But the customers are getting angry because our first-response time has slipped from 2 hours to 24 hours.

**David (Data Eng):** From a data perspective, we have a massive Zendesk archive of past tickets. We could probably train an LLM on those past responses. We also have all our product documentation in Confluence. 

**Sarah (BA):** That’s a great start, David. Could we use a RAG architecture so the AI is dynamically pulling from Confluence rather than fine-tuning a model on static data? That way when docs update, the AI updates.

**David (Data Eng):** Yeah, setting up a vector database pipeline from Confluence to the model is totally feasible. We'd probably use a cheaper model, like Llama 3 or a smaller GPT, for the basic routing, and maybe a heavier model for complex drafting.

**Elena (Legal):** Wait, hang on. If this AI is reading customer emails, what happens if the customer includes sensitive info? Like a social security number or credit card? We cannot have our LLM provider logging that data. We are bound by GDPR and SOC2.

**Sarah (BA):** Excellent point, Elena. So we need a firm non-functional requirement around Data Privacy. David, we'll need a PII scrubbing step *before* the prompt hits any external LLM API. 

**Elena (Legal):** And I also don't want the AI offering refunds or making legal promises. 

**Mark (VP CS):** But sometimes a $10 credit is all it takes to make the customer go away happy! My reps do it all the time.

**Sarah (BA):** Okay, let's define a guardrail here. How about this: The AI can authorize credits up to $15 autonomously based on negative sentiment analysis, but anything higher requires it to draft the response and route it to a human manager for a single-click approval?

**Mark (VP CS):** I can live with that. As long as the AI drafts the email so my manager just has to hit "Approve."

**David (Data Eng):** We can build that "Human-in-the-Loop" workflow. But just so you know, the latency on a complex chain like that—analyze sentiment, check Salesforce, draft email—might take 10-15 seconds of compute time. 

**Sarah (BA):** That's fine for asynchronous email support. We aren't doing a live chat window yet. 

**Sarah (BA):** Okay, my main takeaway is that we aren't just building a chatbot. We are building an Agentic Workflow. I will draft the initial User Stories, the RAG Data Requirements, and the Compliance Guardrails for your review by Thursday.

---
*(End of Transcript)*

## 📝 Practice Exercise:
Use the **[Requirement-Extraction-Agent](../../02-Strategic-Toolkits/Workflow-Prompts/Requirement-Extraction-Agent.md)** prompt to extract formal User Stories, Guardrails, and NFRs from this transcript.