### ➝ Workflow Overview

1. **1⃣ Start with Your Idea**  
   Write your project description as a markdown file (e.g., [idea.md](https://github.com/mikl0s/ai_coding_tools/blob/main/docs/idea.md)).

2. **2⃣ Generate a Project Plan**  
   Use the following prompts to transform your project description into a detailed project plan:
   - Create Plan Prompt: [create-plan.md](https://github.com/mikl0s/ai_coding_tools/blob/main/docs/create-plan.md)  
   - Guidelines Prompt: [guidelines.md](https://github.com/mikl0s/ai_coding_tools/blob/main/docs/guidelines.md)
   - Combine the two prompt above with your a description of your idea - I recommendn iterating on your idea with GPT-4o or Claude.
   - Example "Full Create Plan Prompt": [full-create-plan-prompt.md](https://github.com/mikl0s/ai_coding_tools/blob/main/docs/full-create-plan-prompt.md)  
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
