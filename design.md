# Project Design: AI Career Mentor for Bharat

## System Architecture
- **Client-Server Architecture**
  - Frontend: React / Streamlit for web interface
  - Backend: Python (FastAPI / Flask)
  - AI Module: Hugging Face Transformers for NLP
  - Database: PostgreSQL or MongoDB for user profiles

- **Data Flow**
  1. User sends a query via frontend.
  2. Backend routes the query to AI engine.
  3. AI engine processes the query and generates response.
  4. Response returned to frontend for user display.
  5. User interactions and history stored in the database.

## Technology Stack
- **Frontend:** ReactJS / Streamlit
- **Backend:** Python, FastAPI / Flask
- **AI & NLP:** Hugging Face Transformers, pre-trained language models
- **Database:** PostgreSQL / MongoDB
- **Deployment:** Cloud hosting (AWS / GCP / Azure)

## Database Schema
| Table      | Columns                     | Type            |
|-----------|-----------------------------|----------------|
| Users      | id, name, email, profile    | int, varchar   |
| Resume     | id, user_id, content, feedback | int, int, text, text |
| Skills     | id, user_id, skill_name     | int, int, varchar |
| Interview  | id, user_id, question, answer | int, int, text, text |

## Diagrams
- **System Flow Diagram:** Placeholder for diagram image (e.g., `/images/system_flow.png`)
- **Database ER Diagram:** Placeholder for diagram image (e.g., `/images/db_er.png`)

## Additional Design Notes
- AI engine is modular to allow future expansion (e.g., adding new modules for personality assessment or advanced skill tracking).
- Frontend supports responsive design for mobile and desktop devices.
