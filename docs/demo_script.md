
# 5-Minute AI Assistant Demo Script

## 1. Introduction (0:00–0:40)

Hello everyone.

Today I am presenting an AI Assistant architecture.

It supports document question answering, CRM integration, order information retrieval, unanswerable question handling and email drafting.

## 2. Document Q&A (0:40–1:40)

Demonstrate uploading a document and asking:

"What is the company leave policy?"

Expected: The assistant retrieves relevant information from the document using the Vector Store.

## 3. CRM Tool Call (1:40–2:40)

Ask:

"Show customer details for C101."

Expected: The CRM Tool retrieves customer details using the PostgreSQL data source.

## 4. Refusal (2:40–3:30)

Ask:

"What is the weather on Mars?"

Expected: The assistant responds that it cannot find the requested information.

## 5. Email Draft (3:30–4:20)

Ask:

"Draft a formal leave request email."

Expected: The assistant generates a professional email draft.

## 6. Conclusion (4:20–5:00)

Summarize the architecture:

- UI handles user interaction.
- FastAPI manages requests.
- Vector Store supports document retrieval.
- CRM Tool handles customer queries.
- PostgreSQL stores structured data.

Thank you.