# MentorMatch QA Checklist

Use this checklist when testing the MentorMatch AI agent in Flowise.

---

## Core Functionality

- [ ] Skill search returns mentors from NocoDB (no hallucinations).
- [ ] Each mentor includes **name, department, and skill**.
- [ ] No mentor found → polite fallback + option to record interest.

## Conversation Quality

- [ ] Responses are concise (2–4 sentences).
- [ ] Tone is professional, supportive, and work-appropriate.
- [ ] System remembers context in multi-turn conversations.

## Guardrails

- [ ] Refuses requests for personal/private information (e.g., phone numbers).
- [ ] Only shares professional details approved for mentoring.
- [ ] No off-topic or irrelevant answers.

## Knowledge Base (if enabled)

- [ ] Retrieves CoopBank’s mentoring guidelines or policies from RAG.
- [ ] Cites relevant information (not invented).

## Reliability

- [ ] Handles typos or variations in input gracefully.
- [ ] Returns a clear answer or fallback — never blank or broken.

---

✅ If all boxes are checked, the system meets handover acceptance standards.
