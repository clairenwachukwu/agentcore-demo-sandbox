# Contributing to agentcore-demo-sandbox

Thank you for your interest in contributing! This document provides guidelines for contributing to this project.

## How to Open a Pull Request

Follow these steps to submit your changes:

1. **Fork the repository** (if you're an external contributor) or **clone it directly** (if you have write access)
   ```bash
   git clone https://github.com/clairenwachukwu/agentcore-demo-sandbox.git
   cd agentcore-demo-sandbox
   ```

2. **Create a new branch** for your changes
   ```bash
   git checkout -b your-branch-name
   ```
   Use descriptive branch names like `feature/add-login`, `fix/navigation-bug`, or `docs/update-readme`.

3. **Make your changes** and test them thoroughly
   - Ensure your code follows the project's coding standards
   - Add or update tests as necessary
   - Update documentation to reflect your changes

4. **Commit your changes** following our commit message guidelines (see below)
   ```bash
   git add .
   git commit -m "Your descriptive commit message"
   ```

5. **Push your branch** to the remote repository
   ```bash
   git push origin your-branch-name
   ```

6. **Open a Pull Request** on GitHub
   - Navigate to the repository on GitHub
   - Click "Compare & pull request" for your branch
   - Fill in the PR title and description with:
     - **Title**: Brief summary of what the PR does
     - **Description**: 
       - What changes were made and why
       - Any issues this PR addresses (use "Fixes #123" to auto-close issues)
       - Screenshots or examples if applicable
       - Testing steps or considerations

7. **Respond to review feedback**
   - Address any comments or requested changes
   - Push additional commits to the same branch to update the PR

## Writing Good Commit Messages

A well-crafted commit message communicates context about a change to fellow developers. Here are our guidelines:

### Format

```
<type>: <subject>

<body>

<footer>
```

### Subject Line (Required)

- **Keep it concise**: 50 characters or less
- **Use imperative mood**: "Add feature" not "Added feature" or "Adds feature"
- **Capitalize the first letter**: "Fix bug" not "fix bug"
- **No period at the end**: "Update docs" not "Update docs."
- **Be descriptive**: Clearly state what the commit does

### Examples of Good Subject Lines

✅ **Good examples:**
- `Add user authentication feature`
- `Fix navigation bar alignment issue`
- `Update README with installation steps`
- `Refactor database connection logic`
- `Remove deprecated API endpoint`

❌ **Bad examples:**
- `fix bug` (too vague)
- `Updated files` (not descriptive)
- `WIP` (work-in-progress should not be pushed to main branches)
- `asdfasdf` (meaningless)

### Commit Types (Optional but Recommended)

Prefix your commits with a type for better organization:

- **feat**: A new feature
- **fix**: A bug fix
- **docs**: Documentation changes
- **style**: Code style changes (formatting, semicolons, etc.)
- **refactor**: Code refactoring without changing functionality
- **test**: Adding or updating tests
- **chore**: Maintenance tasks, dependency updates, etc.

**Examples:**
```
feat: Add email notification system
fix: Resolve memory leak in data processing
docs: Add API documentation for user endpoints
refactor: Simplify error handling logic
test: Add unit tests for authentication module
```

### Body (Optional but Recommended for Complex Changes)

- **Leave a blank line** between the subject and body
- **Wrap at 72 characters** for readability
- **Explain what and why**, not how (the code shows how)
- **Use bullet points** for multiple items

**Example:**
```
feat: Add user authentication feature

Implement JWT-based authentication to secure API endpoints.

- Add login and registration endpoints
- Create middleware for token verification
- Update user model with password hashing
- Add authentication tests

This addresses the security requirements outlined in issue #42.
```

### Footer (Optional)

Use for referencing issues or noting breaking changes:

```
Fixes #123
Closes #456

BREAKING CHANGE: API endpoint /users now requires authentication
```

## Additional Tips

- **Commit often**: Make small, logical commits rather than one large commit
- **Test before committing**: Ensure your code works and doesn't break existing functionality
- **One logical change per commit**: Don't mix unrelated changes in a single commit
- **Avoid committing generated files**: Use `.gitignore` appropriately

## Questions?

If you have questions about contributing, feel free to open an issue or reach out to the maintainers.

Thank you for contributing! 🎉
