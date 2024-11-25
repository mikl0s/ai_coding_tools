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
