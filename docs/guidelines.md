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

