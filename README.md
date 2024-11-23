# AI Coding Tools
Various tips and tick, snippets etc. to help use AI coders

Talk to o1-mini
```	
Please generate a project plan for the project below - use epics and stories - use stories with smallest possible scope - more stories with small score is better than few stories with large scope - there is also a guidelines section below, make sure your plan adheres to that as well - use markdown format in a code box - make sure all epics and stories have an unchecked checkbox, so I can update my progress as I move forward - I want to use docker for services where possible like keycloak, posrgresql, redis etc. - Unit testing should be made at each story - not in an epic.

# AI Supervisor App

I want to build a robust app that connects to two LLMs, whether hosted remotely or locally, using common endpoint protocols (e.g., REST, WebSocket). The app will enable one AI to monitor, analyze, and provide dynamic feedback or instructions to the other AI, creating a collaborative or supervisory workflow.

## Key Features

1. **User Authentication**  
   - Utilize **Keycloak** for secure user authentication and role-based access control.
   - Ensure users can safely manage their LLM configurations.

2. **User Interface**  
   - Develop a sleek, modern UI using **Tailwind CSS**.
   - Support both light and dark themes, with the dark theme set as default.

3. **Admin Panel**  
   - Integrate **Forest Admin** for efficient management of user accounts, data, and AI model configurations.

4. **Persistence**  
   - Store LLM configurations, connection settings, logs, and monitoring results in a **PostgreSQL** database.
   - Facilitate data access via a RESTful API.

5. **Session History**  
   - Maintain persistent logs of LLM interactions.
   - Enable users to review and analyze past sessions.

6. **Customizable Instructions**  
   - Allow users to define specific monitoring rules and feedback logic for how the supervisory AI interacts with the primary AI.

7. **Extensibility**  
   - Provide a modular structure to easily add new endpoint types or integrate with additional LLMs.

## Core Technologies
- **Keycloak**: Authentication and role-based access control.
- **Tailwind CSS**: Responsive and modern UI design.
- **Forest Admin**: Admin panel for user and data management.
- **PostgreSQL**: Persistent database storage.
- **REST/WebSocket**: Communication protocols for LLM integration.

## Goals
The app will emphasize security, scalability, and usability, making it an essential tool for advanced AI management workflows.

# AI Coder Guidelines

1. Write **comprehensive unit tests** for every function and module.
2. Follow **TypeScript best practices** and ESLint rules for code quality.
3. Use **descriptive variable and function names** for clarity.
4. Provide **JSDoc comments** for every function, explaining parameters and returns.
5. Ensure **all code is modular** and reusable.
6. Include **error handling** for edge cases and unexpected inputs.
7. Prioritize **efficient algorithms** for processing large PST files.
8. Document every API endpoint with Swagger/OpenAPI.
9. Support **complex queries** for search functionality (e.g., projects, participants).
10. Write **automated tests** for React components using Testing Library.
11. Use **lazy loading** for large datasets where applicable.
12. Encrypt sensitive data at rest and in transit.
13. Ensure **file storage is secure and scalable** using MinIO.
14. Optimize conversational querying with a structured schema for LLM input.
15. Make sure tests run in parallel for both backend and frontend tests.
16. When testing we shouldn't use real services - they should be mocked.
17. Use **TypeORM decorators** for entity definitions and database operations.
18. Implement **proper file validation** using NestJS built-in validators.
19. Use **dependency injection** for better code organization and testing.
20. Follow **NestJS module structure** for organizing related functionality.
```	