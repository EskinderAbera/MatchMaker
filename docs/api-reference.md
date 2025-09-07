# MentorMatch API Reference

MentorMatch integrates **Flowise** with **NocoDB** (employee skills database).  
Below are the key endpoints and how they are used.

---

## 1. Flowise API (Agent Endpoint)

**POST** `/api/v1/prediction/:chatflowId`

- **Description:** Sends a user query to the MentorMatch agent.
- **Headers:**
  - `Authorization: Bearer <FLOWISE_API_KEY>`
  - `Content-Type: application/json`
- **Body:**

```json
{
  "question": "I want to learn project management"
}
```

## 2. NocoDB API (Skills Database)

**GET** `/api/v2/tables/:projectId/:tableId/records`

Description: Fetches employee and skills data from NocoDB.

Headers:

xc-token: <NOCODB_API_KEY>

Query Params Example:
`?where=(skill,eq,Project Management)`

Response Example:

```json
{
  "list": [
    {
      "id": 12,
      "name": "Alemu T.",
      "department": "IT",
      "skills": ["Project Management", "Agile"]
    }
  ]
}
```
