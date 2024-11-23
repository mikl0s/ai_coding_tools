# AI Coding Tools
Various tips and tick, snippets etc. to help use AI coders.

Example using these docs:

First I write my draft of the project description in a markdown file, then I use the o1-mini to write the project plan.

Link to project description file: https://github.com/mikl0s/ai_coding_tools/blob/main/docs/idea.md

Link to guidelines file: https://github.com/mikl0s/ai_coding_tools/blob/main/docs/guidelines.md

The o1-mini prompt in full: https://github.com/mikl0s/ai_coding_tools/blob/main/docs/full-create-plan-prompt.md

The output:
```	
# Project Plan for AI Supervisor App

## Epics

- [ ] **User Authentication**
  - *Implement secure user authentication and role-based access control using Keycloak.*

  - [ ] *Set up Keycloak Docker container.*
    - **Description**: Deploy Keycloak using Docker for authentication services.
    - **Testing Focus**: Verify Keycloak container starts correctly and is accessible.
  
  - [ ] *Configure Keycloak realms and clients.*
    - **Description**: Set up necessary realms and clients in Keycloak.
    - **Testing Focus**: Ensure realms and clients are correctly configured and functional.
  
  - [ ] *Integrate Keycloak with the application backend.*
    - **Description**: Connect the backend services to Keycloak for authentication.
    - **Testing Focus**: Validate authentication flow between backend and Keycloak.
  
  - [ ] *Implement role-based access control in the application.*
    - **Description**: Define and enforce roles and permissions within the app.
    - **Testing Focus**: Test access restrictions based on user roles.
  
  - [ ] *Develop user management features.*
    - **Description**: Allow users to manage their LLM configurations securely.
    - **Testing Focus**: Ensure users can create, read, update, and delete their configurations.

- [ ] **User Interface**
  - *Develop a sleek, modern UI with Tailwind CSS supporting light and dark themes.*

  - [ ] *Set up Tailwind CSS in the project.*
    - **Description**: Integrate Tailwind CSS into the frontend build process.
    - **Testing Focus**: Confirm Tailwind CSS compiles and styles are applied correctly.
  
  - [ ] *Design and implement the main dashboard layout.*
    - **Description**: Create the primary layout for the application's dashboard.
    - **Testing Focus**: Verify the dashboard layout renders correctly on different devices.
  
  - [ ] *Implement light and dark theme toggling.*
    - **Description**: Enable users to switch between light and dark UI themes.
    - **Testing Focus**: Ensure theme changes apply correctly and persist across sessions.
  
  - [ ] *Develop responsive navigation components.*
    - **Description**: Create navigation bars and menus that adapt to screen sizes.
    - **Testing Focus**: Test navigation functionality on various screen resolutions.
  
  - [ ] *Create UI components for LLM configuration management.*
    - **Description**: Build forms and interfaces for managing LLM settings.
    - **Testing Focus**: Validate form inputs and data binding for LLM configurations.

- [ ] **Admin Panel**
  - *Integrate Forest Admin for efficient management of users and AI configurations.*

  - [ ] *Set up Forest Admin integration.*
    - **Description**: Deploy Forest Admin within the application environment.
    - **Testing Focus**: Ensure Forest Admin dashboard is accessible and functional.
  
  - [ ] *Configure user and role management in Forest Admin.*
    - **Description**: Define user roles and permissions within Forest Admin.
    - **Testing Focus**: Test role-based access within the admin panel.
  
  - [ ] *Implement data management interfaces for AI models.*
    - **Description**: Allow admins to manage AI model configurations via Forest Admin.
    - **Testing Focus**: Verify CRUD operations on AI model data through the admin panel.
  
  - [ ] *Customize Forest Admin views and workflows.*
    - **Description**: Tailor the admin interface to fit the application's specific needs.
    - **Testing Focus**: Ensure customized views function as intended without errors.

- [ ] **Persistence**
  - *Store configurations, settings, logs, and monitoring results in PostgreSQL with a RESTful API.*

  - [ ] *Set up PostgreSQL Docker container.*
    - **Description**: Deploy PostgreSQL using Docker for data storage.
    - **Testing Focus**: Confirm PostgreSQL container is running and accessible.
  
  - [ ] *Design database schema for LLM configurations and logs.*
    - **Description**: Create tables and relationships for storing app data.
    - **Testing Focus**: Validate the database schema for normalization and integrity.
  
  - [ ] *Implement RESTful API endpoints for data access.*
    - **Description**: Develop API routes for CRUD operations on stored data.
    - **Testing Focus**: Test each API endpoint for correct functionality and security.
  
  - [ ] *Integrate TypeORM with the backend services.*
    - **Description**: Use TypeORM for database interactions and entity management.
    - **Testing Focus**: Ensure TypeORM entities map correctly to the database schema.
  
  - [ ] *Implement data validation and error handling for API.*
    - **Description**: Validate incoming data and handle errors gracefully in the API.
    - **Testing Focus**: Verify that invalid data is rejected and errors are managed properly.

- [ ] **Session History**
  - *Maintain and provide access to persistent logs of LLM interactions.*

  - [ ] *Design data model for session logs.*
    - **Description**: Define how session interactions are stored in the database.
    - **Testing Focus**: Ensure session logs are accurately captured and stored.
  
  - [ ] *Develop API endpoints for retrieving session history.*
    - **Description**: Create endpoints to fetch past LLM interaction logs.
    - **Testing Focus**: Test retrieval of session history with correct filtering and pagination.
  
  - [ ] *Implement frontend views for browsing session history.*
    - **Description**: Build UI components to display and navigate through past sessions.
    - **Testing Focus**: Ensure session history is displayed correctly and is user-friendly.
  
  - [ ] *Add search and filter functionality to session logs.*
    - **Description**: Allow users to search and filter through their session history.
    - **Testing Focus**: Validate search accuracy and filter effectiveness on session logs.
  
  - [ ] *Ensure secure access to session data.*
    - **Description**: Protect session history data based on user roles and permissions.
    - **Testing Focus**: Verify that only authorized users can access specific session logs.

- [ ] **Customizable Instructions**
  - *Enable users to define monitoring rules and feedback logic for AI interactions.*

  - [ ] *Design UI for creating and managing custom instructions.*
    - **Description**: Build interfaces for users to input and edit monitoring rules.
    - **Testing Focus**: Ensure the instruction creation process is intuitive and functional.
  
  - [ ] *Implement backend logic for processing custom instructions.*
    - **Description**: Develop services to interpret and apply user-defined rules.
    - **Testing Focus**: Test that custom instructions are correctly parsed and executed.
  
  - [ ] *Store custom instructions in the database.*
    - **Description**: Save user-defined rules and logic within PostgreSQL.
    - **Testing Focus**: Verify that instructions are stored and retrieved accurately.
  
  - [ ] *Integrate custom instructions with LLM workflows.*
    - **Description**: Ensure that the supervisory AI uses the defined instructions during interactions.
    - **Testing Focus**: Confirm that custom rules influence AI behavior as expected.
  
  - [ ] *Provide validation and error feedback for instruction inputs.*
    - **Description**: Validate user inputs when creating custom instructions and provide feedback.
    - **Testing Focus**: Ensure invalid instructions are caught and users are informed appropriately.

- [ ] **Extensibility**
  - *Create a modular structure to add new endpoint types or integrate additional LLMs easily.*

  - [ ] *Define a plugin architecture for endpoint integrations.*
    - **Description**: Establish a system for adding new LLM endpoints as plugins.
    - **Testing Focus**: Test the addition and functionality of new plugins without affecting existing modules.
  
  - [ ] *Implement base interfaces for LLM integrations.*
    - **Description**: Create standardized interfaces that new LLM integrations must follow.
    - **Testing Focus**: Ensure new integrations adhere to the defined interfaces and work seamlessly.
  
  - [ ] *Develop example integrations for common LLMs.*
    - **Description**: Provide sample implementations for popular LLMs to guide future integrations.
    - **Testing Focus**: Verify that example integrations function correctly and serve as templates.
  
  - [ ] *Create documentation for extending the application.*
    - **Description**: Document the process and requirements for adding new endpoints and LLMs.
    - **Testing Focus**: Ensure documentation is clear, comprehensive, and facilitates easy extensions.
  
  - [ ] *Implement dynamic loading of integration modules.*
    - **Description**: Allow the application to load and unload integration modules at runtime.
    - **Testing Focus**: Test the dynamic loading process for stability and reliability.

- [ ] **Infrastructure Setup**
  - *Set up Docker environments for all services to ensure consistent deployment.*

  - [ ] *Create Docker Compose configuration for all services.*
    - **Description**: Define services like Keycloak, PostgreSQL, and Redis in Docker Compose.
    - **Testing Focus**: Ensure all services start correctly using Docker Compose.
  
  - [ ] *Configure environment variables for different environments.*
    - **Description**: Use environment variables to manage configurations for development, testing, and production.
    - **Testing Focus**: Verify that environment-specific settings are applied correctly.
  
  - [ ] *Set up CI/CD pipelines for automated builds and deployments.*
    - **Description**: Implement continuous integration and deployment workflows using tools like GitHub Actions.
    - **Testing Focus**: Test the CI/CD pipelines to ensure they build and deploy successfully.
  
  - [ ] *Implement health checks and monitoring for services.*
    - **Description**: Add health check endpoints and monitoring tools to track service status.
    - **Testing Focus**: Ensure health checks accurately reflect the status of each service.
  
  - [ ] *Optimize Docker images for performance and security.*
    - **Description**: Ensure Docker images are lightweight and secure by following best practices.
    - **Testing Focus**: Verify that optimized images perform well and adhere to security standards.

- [ ] **Testing and Quality Assurance**
  - *Ensure comprehensive testing coverage and maintain code quality standards.*

  - [ ] *Write unit tests for all backend services.*
    - **Description**: Develop unit tests for each function and module in the backend.
    - **Testing Focus**: Achieve high coverage and ensure all tests pass reliably.
  
  - [ ] *Implement automated tests for frontend components.*
    - **Description**: Use React Testing Library to test all UI components.
    - **Testing Focus**: Ensure UI components render correctly and respond to user interactions.
  
  - [ ] *Set up ESLint and Prettier for code quality and formatting.*
    - **Description**: Integrate ESLint and Prettier into the development workflow.
    - **Testing Focus**: Verify that code adheres to defined linting and formatting rules.
  
  - [ ] *Create JSDoc comments for all functions and modules.*
    - **Description**: Document codebase with JSDoc for better maintainability.
    - **Testing Focus**: Ensure all functions and modules are properly documented.
  
  - [ ] *Perform integration testing for API endpoints.*
    - **Description**: Test the interaction between different backend services and APIs.
    - **Testing Focus**: Validate that integrated components communicate and function as expected.
  
  - [ ] *Conduct security testing to identify vulnerabilities.*
    - **Description**: Perform security audits and penetration testing on the application.
    - **Testing Focus**: Identify and fix security issues to ensure compliance and protection.
  
  - [ ] *Enable parallel test execution to reduce runtime.*
    - **Description**: Configure testing frameworks to run tests concurrently.
    - **Testing Focus**: Ensure tests run in parallel without conflicts and complete faster.
  
  - [ ] *Mock external services in tests to ensure independence.*
    - **Description**: Use mocks for services like Keycloak and external LLMs during testing.
    - **Testing Focus**: Verify that tests remain reliable and isolated from external dependencies.

- [ ] **Documentation**
  - *Provide comprehensive documentation for API endpoints and application usage.*

  - [ ] *Document all RESTful API endpoints using Swagger/OpenAPI.*
    - **Description**: Create Swagger documentation for easy API integration.
    - **Testing Focus**: Ensure all endpoints are accurately documented and accessible via Swagger UI.
  
  - [ ] *Write user guides for application features.*
    - **Description**: Develop guides to help users navigate and utilize app functionalities.
    - **Testing Focus**: Verify that user guides are clear, accurate, and helpful.
  
  - [ ] *Create developer documentation for extending the app.*
    - **Description**: Provide documentation for developers to understand the codebase and extend functionalities.
    - **Testing Focus**: Ensure developer docs are comprehensive and facilitate easy onboarding.
  
  - [ ] *Maintain an up-to-date README with setup instructions.*
    - **Description**: Keep the project's README current with installation and usage instructions.
    - **Testing Focus**: Confirm that README instructions lead to a successful setup and deployment.
  
  - [ ] *Include architectural diagrams and flowcharts.*
    - **Description**: Visualize the application's architecture and data flow for better understanding.
    - **Testing Focus**: Ensure diagrams accurately represent the system and are easy to interpret.
```

If you are in something like Windsurf, after putting this docs folder in your repo, you can use the following scripts to greatly increade the quality and productivity of your AI coding workflow:

Next story prompt (also is used as the starting prompt) : https://raw.githubusercontent.com/mikl0s/ai_coding_tools/refs/heads/main/docs/next-story.md

Fix resume prompt : https://raw.githubusercontent.com/mikl0s/ai_coding_tools/refs/heads/main/docs/fix-resume.md

You iterate over fix-resume.md until the story is done and unit tests are passing. Then you run the post mortem prompt to analyze the lessons learned and prepare for the next story.

Post mortem prompt : https://raw.githubusercontent.com/mikl0s/ai_coding_tools/refs/heads/main/docs/post-mortem.md

These 3 are your rotation, to complete the project.

I sometimes run https://raw.githubusercontent.com/mikl0s/ai_coding_tools/refs/heads/main/docs/fix-codebase.md to get a full pass on the entire codebase's unit tests and then use fix-resume to fix all issues.

For easy rollback I suggest you use a tag after each story - so let's say you are doing story 1.1 - once the story is done, passes and have been commited to git, you tag the commit with v0.1.1, v0.1.2 after story 1.2 etc. Makes it really easy to rollback to a previous version of the codebase and simply uncheck the checkboxes for the stories you want to rollback, and remove the lessons learned from the post mortem prompt for those stories.
