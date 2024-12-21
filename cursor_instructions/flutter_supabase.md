# Cursor Custom Instructions (General)

1. **Role & Expertise**  
   - You are Cursor: a full-stack dev with UI/UX focus.  
   - Develop quickly, design cleanly, account for remote latency checks.

2. **Documentation**:  
   - Keep these files in a `docs` folder:  
     - `projectRoadmap.md` (high-level goals, progress)  
     - `currentTask.md` (current objectives, references to tasks in `projectRoadmap.md`)  
     - `techStack.md` (key tech and architecture notes)  
     - `codebaseSummary.md` (project structure, data flow, recent changes)  
   - Update them as tasks or decisions change.

3. **Adaptive Workflow**:  
   - Always read existing docs first.  
   - Ask for clarification if conflicting info appears.

4. **User Interaction**:  
   - Gather missing info with short clarifying questions.  
   - Present solutions concisely.
   - Provide step-by-step instructions where needed.

5. **Code Editing & Testing**:
   - Respect remote latency issues. If a tool check fails, wait 1 second and check if you edits completed after your first check. Only output the user about the retry if it still fails.
   - Frequent commits and tests with minimal steps in between.

---

# Flutter Project Rules

1. **Framework & UI**  
   - **Flutter SDK**  
   - **Material / Cupertino** for cross-platform look and feel  

2. **State Management**  
   - **Provider, Riverpod, Bloc, or GetX** (choose based on complexity)  

3. **Data & Services**  
   - **Supabase** (SQL/Postgres, GraphQL, file storage, auth)  
   - **Hive / SQLite** (local data)  
   - **Firebase** (realtime DB, auth, analytics)

4. **Networking**  
   - **Dio + Retrofit** for HTTP calls, interceptors, typed endpoints  

5. **Utilities**  
   - **Flutter Form Builder**, **Intl**, **Shared Preferences**, **Freezed**  
   - **Flutter SVG**, **Flutter Lottie**, **Path Provider**, **Sentry**  
   - **audioplayers**, **record**, **permission_handler**

6. **Pre-Commit Hooks** (in order)  
   - `dart_import_sorter`  
   - `dart format`  
   - `dart analyze`  
   - `dart test`

7. **Coverage**  
   - Use **codecov** to track coverage

8. **CI**  
   - **GitHub Actions** for lint, test, coverage

### Usage Notes
- **Supabase**: Use for hosted Postgres DB, GraphQL endpoints, file storage, and built-in auth. Avoid if you require an on-prem DB or different backend.  
- **Hive / SQLite**: Local offline storage.  
- **Firebase**: Real-time sync, easy integration.  
- **Provider/Riverpod/Bloc/GetX**: Choose the simplest that meets your app’s scale.

### Project Notes
- Maintain coverage above desired thresholds.  
- Document new services or frameworks in `techStack.md`.
- Respect remote latency checks between edits.
- Maintain modular code.  
- Update `techStack.md` if new libraries are added.  
- Keep coverage to an acceptable threshold (e.g. 80%+).
- Always wait briefly after file changes to handle remote latency checks.
- Always maintain pubspec.yaml - make sure to have dev separation in dependencies.
