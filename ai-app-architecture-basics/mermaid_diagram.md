# Basic AI Application Architecture

```mermaid
flowchart TD
    U[User]
    FE1[Frontend - Web or Mobile]
    API[Backend API]
    AI[AI Model]
    BE[Backend - Filters and Logic]
    FE2[Frontend - Response to User]

    U --> FE1
    FE1 -->|Authentication| API
    API -->|Input Validation and Rate Limiting| AI
    AI --> BE
    BE -->|Logging and Monitoring| FE2
