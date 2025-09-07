# MentorMatch Evals — Acceptance Criteria

## What "Good" Looks Like

1. **Accuracy**

   - Mentor suggestions come directly from the NocoDB database.
   - No hallucinated employees or fake skills.

2. **Clarity**

   - Responses are concise (2–4 sentences max).
   - Each mentor suggestion includes name, department, and skill.

3. **Professional Tone**

   - Language is polite, supportive, and work-appropriate.
   - Encourages learning and collaboration.

4. **Resilience**

   - If no mentors are found, system gracefully suggests alternatives (e.g., add skill interest).
   - Handles typos or variations in employee requests.

5. **Privacy & Compliance**

   - Only shares information explicitly allowed (e.g., no personal phone numbers or emails).
   - Respects CoopBank’s internal data protection policies.

6. **Memory**

   - Follow-up questions in the same session use context from earlier queries.

7. **Optional RAG**
   - If configured, knowledge base responses must be relevant and cite internal guidelines.
