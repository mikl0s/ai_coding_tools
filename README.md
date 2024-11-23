# 🚀 AI Coding Tools: Enhance Your Workflow with AI Coders

We believe in the power of collaboration! Any input, suggestions, or contributions are highly welcome to make this project even better. Feel free to open issues, submit pull requests, or simply share your ideas. Together, we can enhance our AI coding workflows!

This repository provides tips, tricks, and snippets to help you effectively use AI-powered coding tools in your projects. By following the provided examples and guidelines, you can significantly improve the quality and productivity of your AI coding workflows.

![GitHub release (latest by date)](https://img.shields.io/github/v/release/mikl0s/ai_coding_tools?cache_bust=1)
![GitHub stars](https://img.shields.io/github/stars/mikl0s/ai_coding_tools)
![GitHub issues](https://img.shields.io/github/issues/mikl0s/ai_coding_tools)

---

## 📚 Table of Contents
- [How to Use These Tools](#how-to-use-these-tools)
  - [Workflow Overview](#workflow-overview)
- [Example Output](#example-output)
- [Suggested Workflow Rotation](#suggested-workflow-rotation)
- [Tips for Productivity](#tips-for-productivity)
- [Tested AI Tools](#tested-ai-tools)

---

## 🚧 How to Use These Tools

### ➝ Workflow Overview

1. **1⃣ Start with Your Idea**  
   Write your project description as a markdown file (e.g., [idea.md](https://github.com/mikl0s/ai_coding_tools/blob/main/docs/idea.md)).

2. **2⃣ Generate a Project Plan**  
   Use the following prompts to transform your project description into a detailed project plan:
   - Guidelines Prompt: [guidelines.md](https://github.com/mikl0s/ai_coding_tools/blob/main/docs/guidelines.md)  
   - Create Plan Prompt: [create-plan.md](https://github.com/mikl0s/ai_coding_tools/blob/main/docs/create-plan.md)  
   - Plan Structure Prompt: [plan.md](https://github.com/mikl0s/ai_coding_tools/blob/main/docs/plan.md)  
   - Full Create Plan Prompt: [full-create-plan-prompt.md](https://github.com/mikl0s/ai_coding_tools/blob/main/docs/full-create-plan-prompt.md)  
   - Example output from **o1-mini**: [Plan.md](https://github.com/mikl0s/ai_coding_tools/blob/main/docs/plan.md)

3. **3⃣ Iterative Development**  
   Utilize the provided prompts and tools to iteratively refine your codebase and address issues:
   - Next Story Prompt: [next-story.md](https://raw.githubusercontent.com/mikl0s/ai_coding_tools/refs/heads/main/docs/next-story.md)  
   - Fix Resume Prompt: [fix-resume.md](https://raw.githubusercontent.com/mikl0s/ai_coding_tools/refs/heads/main/docs/fix-resume.md)  
   - Post-Mortem Prompt: [post-mortem.md](https://raw.githubusercontent.com/mikl0s/ai_coding_tools/refs/heads/main/docs/post-mortem.md)

4. **4⃣ Unit Testing and Codebase Maintenance**  
   For comprehensive testing, run the full codebase evaluation prompt:
   - Fix Codebase Prompt: [fix-codebase.md](https://raw.githubusercontent.com/mikl0s/ai_coding_tools/refs/heads/main/docs/fix-codebase.md)

5. **5⃣ Tagging for Rollback**  
   After completing each story, tag your Git commit for easy versioning.  
   - Example: After finishing story 1.1, tag the commit as `v0.1.1`.  
   - For rollbacks, revert to the desired tag, uncheck relevant story tasks, and adjust lessons learned in the post-mortem.

---

## 💡 Example Output

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

## 🔄 Suggested Workflow Rotation

To complete a project efficiently:
1. **Next Story Prompt**: Start with the current development task.  
2. **Fix Resume Prompt**: Iterate to refine and fix issues until all unit tests pass.  
3. **Post-Mortem Prompt**: Capture lessons learned and prepare for the next story.

---

## ⚡ Tips for Productivity

> **💡 Tip:** Use version tags to manage your project versions effectively.

- **🏷️ Versioning:** Tag each completed story for easy rollback and historical reference.  
- **✅ Testing:** Regularly run the **Fix Codebase Prompt** to ensure the entire codebase remains stable and passes all unit tests.  
- **🤝 Collaboration:** Share the project plan and outputs with your team for transparency and alignment.

---

## 🔍 Tested AI Tools

This toolkit has been tested with several AI-powered development tools, ensuring compatibility and optimizing workflows. Here’s a list of AI tools we have tested, along with their respective links:

- ![Windsurf Editor](https://img.icons8.com/color/48/000000/surfing.png) **Windsurf Editor** - [Windsurf Editor](https://codeium.com/windsurf)
- ![oTToDev](https://img.icons8.com/color/48/000000/artificial-intelligence.png) **oTToDev** - [GitHub Link](https://github.com/coleam00/bolt.new-any-llm)
- ![Cline](https://img.icons8.com/color/48/000000/code.png) **Cline** - [GitHub Link](https://github.com/cline/cline)
- ![Bolt.new](https://img.icons8.com/color/48/000000/bolt.png) **Bolt.new** - [Bolt.new](https://bolt.new)
- ![Aide](https://img.icons8.com/color/48/000000/robot.png) **Aide** - [Aide](https://aide.dev/)
- ![Kodu.ai](https://img.icons8.com/color/48/000000/idea.png) **Kodu.ai** - [Kodu.ai](https://www.kodu.ai/)

---

This repository serves as a complete toolkit for managing AI-driven software projects, helping you iterate quickly, maintain quality, and streamline your development process. **Happy coding!**
