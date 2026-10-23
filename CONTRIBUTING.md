# Contributing to agentcore-demo-sandbox

Thank you for your interest in contributing to this project! This guide will help you understand our contribution process and best practices.

## Table of Contents
- [Opening a Pull Request](#opening-a-pull-request)
- [Writing Good Commit Messages](#writing-good-commit-messages)
- [Code Review Process](#code-review-process)

## Opening a Pull Request

Follow these steps to submit your contribution:

### 1. Fork and Clone the Repository
```bash
# Fork the repository on GitHub, then clone your fork
git clone https://github.com/YOUR_USERNAME/agentcore-demo-sandbox.git
cd agentcore-demo-sandbox
```

### 2. Create a Feature Branch
Always create a new branch for your changes. Never commit directly to `main`.

```bash
git checkout -b feature/your-feature-name
# or
git checkout -b fix/your-bug-fix
```

**Branch naming conventions:**
- `feature/` - for new features
- `fix/` - for bug fixes
- `docs/` - for documentation changes
- `refactor/` - for code refactoring
- `test/` - for adding or updating tests

### 3. Make Your Changes
- Write clear, concise code
- Follow existing code style and conventions
- Add tests for new features when applicable
- Update documentation as needed

### 4. Commit Your Changes
See the [Writing Good Commit Messages](#writing-good-commit-messages) section below.

### 5. Push Your Branch
```bash
git push origin feature/your-feature-name
```

### 6. Open the Pull Request
1. Navigate to the original repository on GitHub
2. Click the "Pull requests" tab
3. Click "New pull request"
4. Click "compare across forks" if you're working from a fork
5. Select your branch as the "compare" branch
6. Fill in the PR template with:
   - **Title**: Clear, concise description (e.g., "Add user authentication feature")
   - **Description**: 
     - What changes were made
     - Why these changes are needed
     - Any relevant issue numbers (e.g., "Fixes #123")
     - Screenshots or examples if applicable
7. Click "Create pull request"

### Pull Request Best Practices
- Keep PRs focused on a single concern
- Keep PRs reasonably small (easier to review)
- Ensure all tests pass before requesting review
- Respond to review feedback promptly
- Keep your branch up to date with `main`

## Writing Good Commit Messages

A well-written commit message helps reviewers understand your changes and makes the project history more useful.

### Format

```
<type>: <subject>

<body>

<footer>
```

### The Subject Line

**Structure:** `<type>: <short summary>`

**Rules:**
- Limit to 50 characters
- Start with a lowercase letter after the type
- Use imperative mood ("add" not "added" or "adds")
- Don't end with a period
- Be specific but concise

**Types:**
- `feat:` - A new feature
- `fix:` - A bug fix
- `docs:` - Documentation changes
- `style:` - Code style changes (formatting, missing semicolons, etc.)
- `refactor:` - Code changes that neither fix bugs nor add features
- `test:` - Adding or updating tests
- `chore:` - Maintenance tasks, dependency updates, etc.
- `perf:` - Performance improvements

**Examples of good subject lines:**
```
feat: add user login functionality
fix: resolve memory leak in data processor
docs: update installation instructions
refactor: simplify error handling logic
test: add unit tests for authentication module
```

### The Body (Optional but Recommended)

- Leave a blank line between the subject and body
- Wrap at 72 characters
- Explain **what** and **why**, not **how**
- Use bullet points for multiple items

**Example:**
```
feat: add user login functionality

- Implement JWT-based authentication
- Add login endpoint with email/password validation
- Include session management with Redis
- Add rate limiting to prevent brute force attacks

This addresses the security requirements outlined in issue #45.
```

### The Footer (Optional)

Use for:
- Referencing issues: `Fixes #123` or `Closes #456`
- Breaking changes: `BREAKING CHANGE: description`
- Co-authors: `Co-authored-by: Name <email>`

### Complete Example

```
fix: resolve race condition in user registration

The registration process was susceptible to race conditions when
multiple requests came in simultaneously with the same email address.
This could result in duplicate user accounts.

Changes:
- Add unique constraint on email field in database
- Implement proper transaction handling
- Add retry logic with exponential backoff

Fixes #234
```

### Quick Tips

✅ **Good commit messages:**
```
feat: add password reset functionality
fix: correct timezone handling in date picker
docs: add API usage examples to README
```

❌ **Bad commit messages:**
```
fixed stuff
WIP
update
asdfasdf
Fixed bug (which bug? what fix?)
```

## Code Review Process

1. **Automated Checks**: All PRs must pass automated tests and linting
2. **Peer Review**: At least one maintainer will review your code
3. **Feedback**: Address any requested changes or questions
4. **Approval**: Once approved, a maintainer will merge your PR
5. **Cleanup**: Delete your feature branch after merging

## Questions?

If you have questions or need help, feel free to:
- Open an issue for discussion
- Reach out to the maintainers
- Comment on your pull request

Thank you for contributing! 🎉
