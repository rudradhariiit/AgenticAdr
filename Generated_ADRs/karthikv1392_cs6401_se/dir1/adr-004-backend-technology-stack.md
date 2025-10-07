---
### ADR-004: Backend Technology Stack

**Status:** Inferred
**Context:** The backend needs to handle API requests, user authentication, data processing from Plaid, business logic for goals and notifications, and communication with the database. The chosen technology should be performant, scalable, and have a strong ecosystem for web development and security.

**Decision:** We will use **Node.js** with the **NestJS** framework, written in **TypeScript**. NestJS provides a structured, opinionated architecture on top of Express.js, making it well-suited for building reliable and maintainable applications.

**Consequences:**
*   **Pros:**
    *   **Language Synergy:** Using TypeScript on both the frontend and backend reduces context switching for developers and enables code sharing (e.g., for data types).
    *   **Performance:** Node.js's non-blocking, event-driven architecture is highly efficient for I/O-bound applications, which is perfect for an API-heavy service that communicates with external services like Plaid and a database.
    *   **Rich Ecosystem:** The NPM registry provides a vast collection of libraries for almost any required functionality.
    *   **Structure & Scalability:** NestJS enforces a solid architectural pattern (heavily inspired by Angular) that promotes modularity and testability, aligning perfectly with our Service-Oriented Monolith decision.
*   **Cons:**
    *   **Single-Threaded:** Node.js is not ideal for CPU-intensive tasks. While not a primary concern for this application, any heavy computational work (e.g., complex report generation) would need to be handled carefully, potentially by offloading to a separate process or service.