### `requirements.md`

# MentorMatch Requirements

## Purpose

CoopBank employees want to learn new skills and find colleagues who can mentor them.  
Currently, knowledge about "who knows what" is scattered across HR systems, LinkedIn, and word of mouth.  
MentorMatch solves this by providing a **central conversational agent** that matches mentees with mentors.

---

## What We’re Building

- A **Flowise-powered chatbot** (MentorMatch AI).
- Integrated with:
  - **NocoDB** (centralized skills/employee database).
  - **Optional Knowledge Base (RAG)** for mentoring policies and FAQs.
- Provides employees with:
  - Mentor recommendations (name, department, skill).
  - Fallback responses when no mentor is available.
  - Guidance on becoming a mentor.

---

## Why We’re Building It

- **Employee Growth:** Helps staff upskill by learning from colleagues.
- **Knowledge Sharing:** Unlocks hidden expertise inside CoopBank.
- **Efficiency:** Saves HR time by automating mentor-mentee matching.
- **Culture:** Strengthens a culture of collaboration and continuous learning.

---

## Key Requirements

1. **Accuracy**

   - Only return mentors that exist in NocoDB.
   - No hallucinated employees.

2. **Security & Privacy**

   - Respect CoopBank’s internal data rules.
   - Share only professional information (no personal contact details).

3. **User Experience**

   - Friendly, professional, concise responses.
   - Context-aware (multi-turn memory).

4. **Extensibility**

   - Allow plugging in new data sources (e.g., HR system).
   - Knowledge base can be expanded with more policies.

5. **Reliability**
   - Clear error handling if database or API is down.
   - Always return either a mentor suggestion or a fallback message.

---

✅ MentorMatch ensures that CoopBank has a **scalable, secure, and user-friendly system** for internal mentoring.
