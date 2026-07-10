```markdown
# openclaw-zero-token Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches you the development patterns and conventions used in the `openclaw-zero-token` repository, a TypeScript backend project built with Express. You'll learn how to structure files, write and organize code, follow commit conventions, and understand how testing is approached in this codebase.

## Coding Conventions

### File Naming
- Use **camelCase** for file names.
  - Example: `userController.ts`, `authMiddleware.ts`

### Import Style
- Use **relative imports** for referencing modules within the project.
  - Example:
    ```typescript
    import { getUser } from './userService';
    ```

### Export Style
- Use **named exports** for all modules.
  - Example:
    ```typescript
    // userService.ts
    export function getUser(id: string) { ... }
    ```

### Commit Messages
- Follow the **Conventional Commits** specification.
- Use the `build` prefix for build-related changes.
  - Example:
    ```
    build: update dependencies for security patch
    ```
- Average commit message length is about 76 characters.

## Workflows

### Code Development
**Trigger:** When adding or updating features or bug fixes  
**Command:** `/develop`

1. Create or update files using camelCase naming.
2. Use relative imports and named exports.
3. Write clear, conventional commit messages (e.g., `build: add new endpoint for user login`).
4. Ensure code is organized and follows the project's style.

### Testing
**Trigger:** When writing or updating tests  
**Command:** `/test`

1. Create test files with the pattern `*.test.*` (e.g., `userService.test.ts`).
2. Place tests alongside or near the modules they cover.
3. Use the project's chosen (unknown) testing framework.
4. Run tests and ensure all pass before committing.

## Testing Patterns

- Test files follow the `*.test.*` naming convention.
  - Example: `authMiddleware.test.ts`
- The specific testing framework is not detected, but tests are organized in dedicated files.
- Place test files near the code they are testing for clarity and maintainability.

## Commands
| Command   | Purpose                                         |
|-----------|-------------------------------------------------|
| /develop  | Start a new feature or bugfix with conventions  |
| /test     | Write or update tests using the correct patterns |
```
