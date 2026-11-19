
# AI Assistant – Documentation and Demo Project

## 1. Project Purpose

This project demonstrates the documentation, architecture and demo preparation of an AI-powered assistant.

The assistant is designed to support:

- Document question answering
- CRM customer information retrieval
- Order information retrieval
- Handling unanswerable questions
- Email draft generation

## 2. System Architecture

The system contains the following components:

- UI: User interacts with the assistant.
- FastAPI: Handles incoming API requests.
- Vector Store: Stores document embeddings for retrieval.
- CRM Tool: Retrieves customer information.
- PostgreSQL: Stores customer and order information.

See [Architecture Diagram](docs/architecture.mmd).

## 3. Technology Stack

| Technology | Purpose |
|---|---|
| Python | Backend development |
| FastAPI | API framework |
| Vector Store | Document retrieval |
| PostgreSQL | Database |
| Git | Version control |
| GitHub | Source code repository |

## 4. Architecture Flow

1. User submits a question through the UI.
2. FastAPI receives the request.
3. FastAPI identifies the required operation.
4. Document questions are handled using the Vector Store.
5. Customer questions are handled by the CRM Tool.
6. Customer and order data are stored in PostgreSQL.
7. The API returns the response to the UI.

## 5. Setup Instructions

### Prerequisites

- Python 3.10 or higher
- Visual Studio Code
- Git
- PostgreSQL (for database integration)

### Clone Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd readme-demo-project
```

### Create Virtual Environment

```bash
python -m venv venv
```

### Activate Environment

Windows PowerShell:

```powershell
.\venv\Scripts\Activate.ps1
```

### Install Dependencies

```bash
python -m pip install -r requirements.txt
```

## 6. Environment Variables

Create a `.env` file for environment-specific configuration.

Example:

```env
DATABASE_URL=postgresql://username:password@localhost:5432/assistant_db
CRM_API_KEY=your_crm_api_key
VECTOR_STORE_PATH=./vector_store
```

Do not commit real passwords or API keys to GitHub.

## 7. Example Questions

### Document Q&A
- What is the company leave policy?
- Summarize the uploaded document.

### CRM
- Show customer details for C101.

### Order
- What is the status of order O101?

### Unanswerable Question
- What is the weather on Mars?

### Email Draft
- Draft a formal leave request email.

## 8. Demo Plan

The 5-minute demonstration includes:

1. Introduction and application overview.
2. Document question answering.
3. CRM tool call.
4. Refusal of an unanswerable question.
5. Email draft generation.

See [Demo Script](docs/demo_script.md).

## 9. Future Enhancements

- Authentication and authorization
- Real-time CRM integration
- Vector database integration
- Monitoring and logging
- Improved UI

## 10. Submission

Deliverables:

- README documentation
- Architecture diagram
- Five-minute demo
- Two-minute backup demo video
- GitHub Pull Request and merge