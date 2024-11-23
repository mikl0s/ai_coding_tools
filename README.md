# AI Coding Tools
Various tips and tick, snippets etc. to help use AI coders.

Example using these docs:

First I write my draft of the project description in a markdown file, then I use the o1-mini to write the project plan.

Link to project description file: https://github.com/mikl0s/ai_coding_tools/blob/main/docs/idea.md

Link to guidelines file: https://github.com/mikl0s/ai_coding_tools/blob/main/docs/guidelines.md

The o1-mini prompt in full: https://github.com/mikl0s/ai_coding_tools/blob/main/docs/full-create-plan-prompt.md

The output: https://github.com/mikl0s/ai_coding_tools/blob/main/docs/plan.md
```Markdown
Example output:

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

If you are in something like Windsurf, after putting this docs folder in your repo, you can use the following scripts to greatly increade the quality and productivity of your AI coding workflow:

Next story prompt (also is used as the starting prompt) : https://raw.githubusercontent.com/mikl0s/ai_coding_tools/refs/heads/main/docs/next-story.md

Fix resume prompt : https://raw.githubusercontent.com/mikl0s/ai_coding_tools/refs/heads/main/docs/fix-resume.md

You iterate over fix-resume.md until the story is done and unit tests are passing. Then you run the post mortem prompt to analyze the lessons learned and prepare for the next story.

Post mortem prompt : https://raw.githubusercontent.com/mikl0s/ai_coding_tools/refs/heads/main/docs/post-mortem.md

These 3 are your rotation, to complete the project.

I sometimes run https://raw.githubusercontent.com/mikl0s/ai_coding_tools/refs/heads/main/docs/fix-codebase.md to get a full pass on the entire codebase's unit tests and then use fix-resume to fix all issues.

For easy rollback I suggest you use a tag after each story - so let's say you are doing story 1.1 - once the story is done, passes and have been commited to git, you tag the commit with v0.1.1, v0.1.2 after story 1.2 etc. Makes it really easy to rollback to a previous version of the codebase and simply uncheck the checkboxes for the stories you want to rollback, and remove the lessons learned from the post mortem prompt for those stories.
