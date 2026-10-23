# Contributing to AgentCore Demo Sandbox

Thank you for your interest in contributing to this project! This document provides guidelines to help you contribute effectively.

## Table of Contents

- [Opening a Pull Request](#opening-a-pull-request)
- [Writing Good Commit Messages](#writing-good-commit-messages)
- [Code Review Process](#code-review-process)

## Opening a Pull Request

Follow these steps to submit your changes:

### 1. Fork and Clone the Repository

```bash
git clone https://github.com/clairenwachukwu/agentcore-demo-sandbox.git
cd agentcore-demo-sandbox
```

### 2. Create a New Branch

Always create a new branch for your changes. Use a descriptive name that reflects the work you're doing:

```bash
git checkout -b feature/your-feature-name
```

Branch naming conventions:
- `feature/` - for new features
- `fix/` - for bug fixes
- `docs/` - for documentation updates
- `refactor/` - for code refactoring
- `test/` - for adding or updating tests

### 3. Make Your Changes

- Write clean, readable code
- Follow the existing code style and conventions
- Add tests for new features when applicable
- Update documentation as needed

### 4. Commit Your Changes

See the [Writing Good Commit Messages](#writing-good-commit-messages) section below for guidelines.

### 5. Push Your Branch

```bash
git push origin feature/your-feature-name
```

### 6. Open a Pull Request

1. Go to the repository on GitHub
2. Click the "Pull requests" tab
3. Click "New pull request"
4. Select your branch as the compare branch
5. Fill in the pull request template with:
   - **Title**: A clear, concise summary of your changes
   - **Description**: What changes were made and why
   - **Related Issues**: Link any related issues using `#issue-number`
   - **Testing**: Describe how you tested your changes
   - **Screenshots**: Add screenshots for UI changes (if applicable)

### Pull Request Checklist

Before submitting your PR, ensure:

- [ ] Code follows the project's style guidelines
- [ ] All tests pass
- [ ] New tests added for new features
- [ ] Documentation has been updated
- [ ] Commit messages follow the guidelines below
- [ ] No merge conflicts with the main branch

## Writing Good Commit Messages

Good commit messages make it easier to understand the project's history and the reasoning behind changes.

### Commit Message Format

```
<type>: <subject>

<body>

<footer>
```

### Subject Line

The subject line should:

- **Be concise**: Aim for 50 characters or less
- **Use imperative mood**: "Add feature" not "Added feature" or "Adds feature"
- **Start with a capital letter**
- **Not end with a period**
- **Clearly describe what the commit does**

### Type Prefix

Start your subject line with one of these types:

- `feat:` - A new feature
- `fix:` - A bug fix
- `docs:` - Documentation changes
- `style:` - Code style changes (formatting, semicolons, etc.)
- `refactor:` - Code refactoring without changing functionality
- `test:` - Adding or updating tests
- `chore:` - Maintenance tasks, dependency updates, etc.
- `perf:` - Performance improvements

### Body (Optional)

The body should:

- Be separated from the subject by a blank line
- Explain **what** and **why**, not **how**
- Wrap lines at 72 characters
- Use bullet points for multiple items

### Footer (Optional)

The footer can include:

- References to issues: `Closes #123` or `Fixes #456`
- Breaking changes: `BREAKING CHANGE: description`

### Good Commit Message Examples

#### Example 1: Simple feature
```
feat: Add user authentication endpoint

Implement JWT-based authentication for API access.
Users can now log in and receive a token for
authenticated requests.

Closes #42
```

#### Example 2: Bug fix
```
fix: Resolve memory leak in data processor

The processor was not releasing resources after
completing tasks, causing memory to grow unbounded
over time.

Fixes #78
```

#### Example 3: Documentation
```
docs: Add installation instructions to README

Include step-by-step setup guide for local development
and deployment options.
```

#### Example 4: Refactoring
```
refactor: Extract validation logic into separate module

Move validation functions from controller to a dedicated
validator module for better code organization and reusability.
```

### Poor Commit Message Examples

❌ `fixed stuff` - Too vague, doesn't explain what was fixed

❌ `Updated code.` - Doesn't describe what changed or why

❌ `WIP` - Work in progress commits should be squashed before merging

❌ `asdfasdf` - Not descriptive at all

❌ `Fixed bug in the authentication system that was causing users to not be able to log in properly when using special characters` - Too long for subject line (should be split into subject and body)

## Code Review Process

Once you've submitted your pull request:

1. **Automated checks** will run (if configured)
2. **Maintainers will review** your code
3. You may be asked to make changes
4. Once approved, your PR will be merged

### Responding to Feedback

- Be open to constructive criticism
- Make requested changes in new commits
- Push updates to your branch (the PR will update automatically)
- Respond to comments to keep the conversation flowing

## Questions?

If you have questions or need help, please:

- Open an issue for discussion
- Reach out to the maintainers
- Check existing issues and pull requests for similar questions

Thank you for contributing! 🎉
