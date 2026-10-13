# AGENTS.md

## Project Overview

Build a simple, interactive task management web application that allows users to create, view, edit, complete, and delete tasks. The purpose of this project is to demonstrate how an AI coding agent can use an `AGENTS.md` file to follow project instructions, coding standards, and development guidelines while building software.

The application should prioritize simplicity, usability, maintainability, and reliable functionality over unnecessary complexity.

## Functional Requirements

1. **Task Creation:**
   - Allow users to create a new task.
   - Each task must have a title.
   - Allow users to provide an optional description.
   - Validate that task titles are not blank.
   - Trim leading and trailing whitespace from user inputs.

2. **Task Display:**
   - Display all created tasks in a clear, organized task list.
   - Show each task's title, description when provided, and completion status.
   - Display a helpful message when no tasks exist.

3. **Task Editing:**
   - Allow users to edit an existing task's title and description.
   - Validate updated task titles to ensure they are not blank.
   - Preserve the task's existing completion status when editing other fields.

4. **Task Completion:**
   - Allow users to mark a task as complete or incomplete.
   - Clearly distinguish completed tasks from incomplete tasks.
   - Update the displayed task status immediately after a change.

5. **Task Deletion:**
   - Allow users to delete existing tasks.
   - Update the task list immediately after deletion.
   - Prevent deleted tasks from appearing in the active task list.

6. **User Interface:**
   - Provide a simple, intuitive, and responsive web interface.
   - Use consistent spacing, typography, buttons, and form controls.
   - Provide clear feedback for successful actions and validation errors.
   - Keep the interface easy to navigate on desktop and mobile devices.

## Technical Guidelines

- **Language and Environment:** Use the programming language, framework, and tools selected for the project. Prefer the existing repository configuration over introducing new technologies unnecessarily.
- **Architecture:** Organize the application into logical components and modules. Separate user interface code, task-related business logic, and data access when appropriate.
- **Data Model:** Each task should have a unique identifier, a title, an optional description, a completion status, and timestamps when appropriate.
- **Data Persistence:** Use the project's selected storage solution. If persistence has not yet been implemented, keep the design flexible enough to support saving tasks between sessions in a future iteration.
- **Dependencies:** Prefer existing dependencies and standard framework capabilities. Add third-party packages only when they provide clear value.
- **Code Quality:**
  - Use descriptive variable, function, and component names.
  - Keep functions and components small and focused.
  - Avoid unnecessary duplication and overly complicated implementations.
  - Follow the established formatting and naming conventions of the repository.
  - Add comments and documentation when they clarify non-obvious behavior.
  - Handle errors gracefully and provide useful feedback to users.
- **Accessibility:** Use semantic HTML, properly labeled form controls, keyboard-accessible interactions, and sufficient visual contrast.
- **Security:** Validate user input and avoid exposing secrets, credentials, or sensitive configuration in source code.
- **Version Control:** Keep changes focused and use descriptive Git commit messages.
- **AI Coding Agent:** Read and follow this file before making changes. Inspect the existing codebase before implementing new features. Explain significant implementation decisions and avoid modifying unrelated functionality.

## Development Workflow

1. **Inspect:** Review the existing project structure, dependencies, configuration, and relevant source files before making changes.
2. **Plan:** Break requested features into small, manageable implementation steps.
3. **Implement:** Make the smallest reasonable changes needed to satisfy the requirements.
4. **Test:** Verify the affected functionality and check for regressions.
5. **Review:** Look for bugs, duplicated logic, accessibility issues, and unnecessary complexity.
6. **Document:** Update the README and other documentation when setup instructions, features, or dependencies change.

Do not assume a feature works simply because the code has been written. Run the available checks and manually verify important user workflows when possible.

## Testing Requirements

- Verify that a user can create a task with a valid title.
- Verify that blank or whitespace-only titles are rejected.
- Verify that task titles and descriptions are trimmed appropriately.
- Verify that tasks display their correct details and completion status.
- Verify that tasks can be edited without unintentionally changing their completion status.
- Verify that tasks can be marked complete and incomplete.
- Verify that tasks can be deleted.
- Verify that the application handles an empty task list correctly.
- Verify that the application starts successfully using the documented development command.
- Test persistence across page reloads if persistence is implemented.
- Run available automated tests, linting, and type checks before considering the work complete.

## Definition of Done

A feature is complete when:

- Its behavior meets the applicable functional requirements.
- The application runs without errors related to the changes.
- Input validation and error handling work as expected.
- The interface remains clear and usable on desktop and mobile devices.
- Relevant tests have been run and pass.
- No unrelated functionality has been broken.
- Documentation is updated when necessary.

The project is considered complete when users can create, view, edit, complete, and delete tasks through the web interface and the core workflows have been tested.

## Future Work

Potential enhancements include:

- Task priorities such as low, medium, and high.
- Task categories or tags.
- Filtering tasks by completion status.
- Sorting tasks by creation date, priority, or title.
- Persistent storage across browser sessions.
- Automated unit and integration tests.
- Improved accessibility and user experience.
- A demonstration explaining how the AI coding agent uses `AGENTS.md` to guide development.
