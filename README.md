
# AI Coding Tools: Enhance Your Workflow with AI Coders

This repository provides tips, tricks, and snippets to help you effectively use AI-powered coding tools in your projects. By following the provided examples and guidelines, you can significantly improve the quality and productivity of your AI coding workflows.

---

## How to Use These Tools

### Workflow Overview

1. **Start with Your Idea**  
   Write your project description as a markdown file (e.g., [idea.md](https://github.com/mikl0s/ai_coding_tools/blob/main/docs/idea.md)).

2. **Generate a Project Plan**  
   Use the following prompts to transform your project description into a detailed project plan:
   - **Guidelines Prompt**: [guidelines.md](https://github.com/mikl0s/ai_coding_tools/blob/main/docs/guidelines.md)  
   - **Create Plan Prompt**: [create-plan.md](https://github.com/mikl0s/ai_coding_tools/blob/main/docs/create-plan.md)  
   - **Plan Structure Prompt**: [plan.md](https://github.com/mikl0s/ai_coding_tools/blob/main/docs/plan.md)  

   These are combined into a single **Full Create Plan Prompt**: [full-create-plan-prompt.md](https://github.com/mikl0s/ai_coding_tools/blob/main/docs/full-create-plan-prompt.md).  
   - **Example output**: [Plan.md](https://github.com/mikl0s/ai_coding_tools/blob/main/docs/plan.md)

3. **Iterative Development**  
   Utilize the provided prompts and tools to iteratively refine your codebase and address issues:
   - **Next story prompt**: [next-story.md](https://raw.githubusercontent.com/mikl0s/ai_coding_tools/refs/heads/main/docs/next-story.md)  
   - **Fix resume prompt**: [fix-resume.md](https://raw.githubusercontent.com/mikl0s/ai_coding_tools/refs/heads/main/docs/fix-resume.md)  
   - **Post-mortem prompt**: [post-mortem.md](https://raw.githubusercontent.com/mikl0s/ai_coding_tools/refs/heads/main/docs/post-mortem.md)

4. **Unit Testing and Codebase Maintenance**  
   For comprehensive testing, run the full codebase evaluation prompt:
   - **Fix codebase prompt**: [fix-codebase.md](https://raw.githubusercontent.com/mikl0s/ai_coding_tools/refs/heads/main/docs/fix-codebase.md)

5. **Tagging for Rollback**  
   After completing each story, tag your Git commit for easy versioning.  
   - Example: After finishing story 1.1, tag the commit as `v0.1.1`.  
   - For rollbacks, revert to the desired tag, uncheck relevant story tasks, and adjust lessons learned in the post-mortem.

---

### Example Output

Here’s an example of a generated project plan:

```markdown
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
```

---

### Suggested Workflow Rotation

To complete a project efficiently:
1. Use the **Next Story Prompt** as a starting point for the current development task.  
2. Iterate using the **Fix Resume Prompt** to refine and fix issues until all unit tests pass.  
3. Run the **Post-Mortem Prompt** after each story to capture lessons learned and prepare for the next story.

---

### Tips for Productivity

- **Versioning:** Tag each completed story for easy rollback and historical reference.  
- **Testing:** Regularly run the **Fix Codebase Prompt** to ensure the entire codebase remains stable and passes all unit tests.  
- **Collaboration:** Share the project plan and outputs with your team for transparency and alignment.

---

This repository serves as a complete toolkit for managing AI-driven software projects, helping you iterate quickly, maintain quality, and streamline your development process. Happy coding!
