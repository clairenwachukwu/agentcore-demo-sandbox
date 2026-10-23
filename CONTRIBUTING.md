# Contributing to AgentCore Demo Sandbox

Thank you for your interest in contributing to this project! This guide will help you understand our process for submitting changes.

## How to Open a Pull Request

Follow these steps to contribute code changes:

### 1. Fork and Clone the Repository

```bash
# Fork the repository on GitHub first, then clone your fork
git clone https://github.com/YOUR_USERNAME/agentcore-demo-sandbox.git
cd agentcore-demo-sandbox
```

### 2. Create a New Branch

Always create a new branch for your changes. Never commit directly to the `main` branch.

```bash
git checkout -b feature/your-feature-name
```

Branch naming conventions:
- `feature/` - for new features
- `fix/` - for bug fixes
- `docs/` - for documentation updates
- `refactor/` - for code refactoring

### 3. Make Your Changes

Make your code changes, following the project's coding standards and best practices.

### 4. Test Your Changes

Ensure your changes work as expected and don't break existing functionality.

### 5. Commit Your Changes

See the "Writing Good Commit Messages" section below for guidance on commit messages.

```bash
git add .
git commit -m "Your descriptive commit message"
```

### 6. Push Your Branch

```bash
git push origin feature/your-feature-name
```

### 7. Open a Pull Request

1. Navigate to the original repository on GitHub
2. Click the "New Pull Request" button
3. Select your branch as the source and `main` as the target
4. Fill in the PR title and description (see below)
5. Submit the pull request

### Pull Request Title and Description

**Title:** Should be clear and concise, summarizing the change in one line.

Example titles:
- `Add user authentication feature`
- `Fix null pointer exception in data processor`
- `Update README with installation instructions`

**Description:** Should include:
- What changes were made
- Why the changes were necessary
- Any related issue numbers (e.g., "Fixes #123")
- Testing performed
- Screenshots (if UI changes)

Example PR description:
```
## Changes
- Added CONTRIBUTING.md file with contribution guidelines
- Documented commit message best practices
- Outlined pull request process

## Reason
To help new contributors understand how to contribute effectively to the project.

## Testing
- Verified markdown renders correctly on GitHub
- Reviewed for clarity and completeness
```

## Writing Good Commit Messages

A good commit message helps others understand what changed and why. Follow these guidelines:

### Format

```
<type>: <subject>

<body>

<footer>
```

### The Seven Rules of a Great Commit Message

1. **Separate subject from body with a blank line**
2. **Limit the subject line to 50 characters**
3. **Capitalize the subject line**
4. **Do not end the subject line with a period**
5. **Use the imperative mood in the subject line** ("Add feature" not "Added feature")
6. **Wrap the body at 72 characters**
7. **Use the body to explain what and why vs. how**

### Commit Message Types

- `feat:` - A new feature
- `fix:` - A bug fix
- `docs:` - Documentation changes
- `style:` - Code style changes (formatting, missing semicolons, etc.)
- `refactor:` - Code refactoring without changing functionality
- `test:` - Adding or updating tests
- `chore:` - Maintenance tasks, dependency updates, etc.

### Good Examples

```
feat: Add user login functionality

Implement JWT-based authentication with login endpoint.
Users can now authenticate using email and password.

Fixes #42
```

```
fix: Prevent race condition in data loader

Add mutex lock to ensure thread-safe access to shared resource.
This resolves intermittent crashes reported in production.
```

```
docs: Update installation instructions

Add prerequisites section and clarify Node.js version requirement.
```

### Bad Examples

❌ `fixed stuff` - Too vague
❌ `Updated files` - Doesn't explain what changed
❌ `WIP` - Work in progress should not be in main branch
❌ `asdfasdf` - Not descriptive at all
❌ `Fixed bug in the login system and also updated some documentation and refactored code` - Too much in one commit

### Tips

- **Make atomic commits:** Each commit should represent one logical change
- **Commit often:** Small, frequent commits are better than large, infrequent ones
- **Write for your future self:** You'll thank yourself later when debugging
- **Reference issues:** Include issue numbers when applicable (e.g., "Fixes #123")

## Code Review Process

Once you've opened a pull request:

1. A maintainer will review your changes
2. They may request changes or ask questions
3. Make any requested updates by pushing new commits to your branch
4. Once approved, a maintainer will merge your PR

## Questions?

If you have questions about contributing, feel free to open an issue or reach out to the maintainers.

Thank you for contributing! 🎉
