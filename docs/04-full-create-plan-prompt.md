# Prompt

Please generate a detailed project plan based on the project description below. Structure the plan using epics and stories. Follow these guidelines:

1. **Stories Scope**:  
   - Break down each epic into the smallest possible stories.  
   - Prioritize having more small stories over fewer large ones.
   - Ensure the plan adheres to the guidelines section below.
   - Include a one line description of each story.
   - Include a one line summary of the epic.
   - Include a one line of focus for testing of that story.

2. **Guidelines Compliance**:  
   - There is a guidelines section included below. Ensure the plan strictly adheres to those guidelines.  

3. **Format**:  
   - Use **Markdown** enclosed in a code block.  
   - Include **unchecked checkboxes** (`- [ ]`) for all epics and stories, so I can track progress.  

4. **Technology Stack**:  
   - Use Docker for services wherever possible (e.g., Keycloak, PostgreSQL, Redis).  

5. **Unit Testing**:  
   - Ensure unit tests are included for each story, not at the epic level.  

**Plan Structure**:  
- Begin with a list of epics.  
- Under each epic, list detailed stories with the smallest possible scope.  

**Output the plan in Markdown format, in a code block.**



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

## Code Quality
1. Write **comprehensive unit tests** for every function and module to ensure robust functionality.
2. Follow **TypeScript best practices** and adhere to **ESLint rules** for maintaining code quality.
3. Use **descriptive variable and function names** to enhance clarity and readability.
4. Provide **JSDoc comments** for all functions, detailing parameters, return types, and functionality.

## Architecture and Modularity
5. Ensure **all code is modular**, reusable, and adheres to SOLID principles.
6. Use **dependency injection** for better code organization, scalability, and testability.
7. Follow **NestJS module structure** to organize related functionality logically.
8. Use **TypeORM decorators** for defining entities and managing database operations.

## Error Handling and Security
9. Implement **error handling** to account for edge cases and unexpected inputs.
10. Encrypt sensitive data **at rest and in transit** for security compliance.
11. Validate file uploads using **NestJS built-in validators** to prevent malicious uploads.

## Performance and Optimization
12. Prioritize **efficient algorithms** for handling large PST files and data sets.
13. Use **lazy loading** techniques to optimize rendering for large datasets.
14. Optimize **conversational querying** by designing a structured schema tailored for LLM input.

## Documentation and Testing
15. Document all API endpoints using **Swagger/OpenAPI** for easy integration and clarity.
16. Write **automated tests** for React components with **React Testing Library**.
17. Mock real services in tests to ensure independence and faster execution.
18. Enable **parallel test execution** for backend and frontend tests to reduce runtime.

## Features and Functionality
19. Support **complex queries** for search functionality, including filtering by projects, participants, and other attributes.
20. Ensure **file storage is secure and scalable** using **MinIO** as the backend solution.

## Best Practices
21. Maintain a clear separation of concerns in modules and codebase.
22. Avoid hardcoding configurations; use environment variables for flexibility.
23. Always consider scalability and future maintainability when designing components or architecture.

