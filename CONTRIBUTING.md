# Contributing to RevoiceChat

Thank you for your interest in contributing to RevoiceChat! We welcome contributions from everyone, whether you're fixing a typo, reporting a bug, or implementing a new feature.

## 📋 Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Getting Started](#getting-started)
- [Development Workflow](#development-workflow)
- [Coding Standards](#coding-standards)
- [Commit Guidelines](#commit-guidelines)
- [Pull Request Process](#pull-request-process)
- [Community](#community)

---

## 📜 Code of Conduct

This project and everyone participating in it is governed by our Code of Conduct. By participating, you are expected to uphold this code. Please report unacceptable behavior to [hello@revoicechat.org](mailto:hello@revoicechat.org).

**In short:**
- Be respectful and inclusive
- Be patient and welcoming
- Be collaborative
- Focus on what is best for the community

---

## 🤝 How Can I Contribute?

### Reporting Bugs

Before creating a bug report, please check the [existing issues](https://github.com/revoicechat/revoicechat/issues) to avoid duplicates.

**When reporting a bug, please include:**
- A clear and descriptive title
- Steps to reproduce the issue
- Expected behavior vs. actual behavior
- Screenshots or error messages (if applicable)
- Your environment (OS, browser, RevoiceChat version)

**Use the github `Bug Report` template**

### Suggesting Features

We love new ideas! Before suggesting a feature:
- Check if it's already been suggested
- Ensure it aligns with the project's goals
- Provide a clear use case

**Use the github `Fearure Request` template**

### Improving Documentation

Documentation improvements are always welcome! This includes:
- Fixing typos or clarifying instructions
- Adding examples
- Translating documentation
- Writing tutorials or guides

---

## 🚀 Getting Started

### Prerequisites

Make sure you have installed:
- Git
- Docker
- For the Core server
  - PostgreSQL (v14 or higher)
  - Java 21
- For the Media server
  - PHP
- For the Front
  - If you run the webapp : nothing particular
  - If you run the desktop app :
    - Node JS
    - Rust

### Setting Up Your Development Environment

refer to the setup section of each repository

- 📄 **Main repository:** [revoicechat/revoicechat](https://github.com/revoicechat/revoicechat)
- 🌐 **Core Server:** [revoicechat/ReVoiceChat-CoreServer](https://github.com/revoicechat/ReVoiceChat-CoreServer)
- 🖼️ **Media Server:** [revoicechat/ReVoiceChat-MediaServer](https://github.com/revoicechat/ReVoiceChat-MediaServer)
- 💻 **Web Client:** [revoicechat/ReVoiceChat-WebClient](https://github.com/revoicechat/ReVoiceChat-WebClient)
- 💻 **Admin Dashboard:** [revoicechat/ReVoiceChat-AdminDashboard](https://github.com/revoicechat/ReVoiceChat-AdminDashboard)

---

## 📝 Coding Standards

### General Principles

- **Keep it simple** - Write clear, straightforward code
- **DRY (Don't Repeat Yourself)** - Avoid code duplication
- **KISS (Keep It Simple, Stupid)** - Avoid unnecessary complexity
- **Write self-documenting code** - Use clear variable and function names

### Comments

- Write comments for complex logic
- Avoid obvious comments
- Use JSDoc for functions and classes

```javascript
/**
 * Calculates the user's age based on their birth date
 * @param {Date} birthDate - The user's birth date
 * @returns {number} The calculated age in years
 */
const calculateAge = (birthDate) => {
  const today = new Date();
  const age = today.getFullYear() - birthDate.getFullYear();
  return age;
};
```

---

## 💬 Commit Guidelines

We follow [Conventional Commits](https://www.conventionalcommits.org/) for clear and consistent commit messages.

### Format

```
<type>(<scope>): <subject>

<body>

<footer>
```

### Types

- **feat**: A new feature
- **fix**: A bug fix
- **docs**: Documentation changes
- **style**: Code style changes (formatting, missing semicolons, etc.)
- **refactor**: Code refactoring without changing functionality
- **perf**: Performance improvements
- **test**: Adding or updating tests
- **chore**: Maintenance tasks (dependencies, build config, etc.)
- **ci**: CI/CD changes

### Examples

```bash
feat(auth): add OAuth2 authentication

fix(chat): resolve message duplication issue

docs(readme): update installation instructions

refactor(api): simplify error handling logic

test(user): add unit tests for user service
```

### Tips

- Use imperative mood ("add" not "added" or "adds")
- Don't capitalize the first letter
- No period at the end of the subject line
- Keep the subject line under 50 characters
- Add a body if more context is needed

---

## 🔀 Pull Request Process

### Before Submitting

- ✅ All tests pass
- ✅ Code follows our style guidelines
- ✅ Documentation is updated
- ✅ Commits follow our commit guidelines
- ✅ Branch is up to date with main

### Submitting a Pull Request

1. **Push your branch to your fork**
   ```bash
   git push origin feature/your-feature-name
   ```

2. **Create a Pull Request on GitHub**
    - Go to the original repository
    - Click "New Pull Request"
    - Select your branch
    - Fill in the PR template

3. **PR Template**
   ```markdown
   ## Description
   Brief description of changes

   ## Type of Change
   - [ ] Bug fix
   - [ ] New feature
   - [ ] Breaking change
   - [ ] Documentation update

   ## Related Issues
   Closes #123

   ## Testing
   How has this been tested?

   ## Screenshots (if applicable)
   Add screenshots here

   ## Checklist
   - [ ] Tests pass
   - [ ] Code follows style guidelines
   - [ ] Documentation updated
   - [ ] No breaking changes
   ```

### Review Process

- A maintainer will review your PR
- Address any feedback or requested changes
- Once approved, a maintainer will merge your PR
- Your contribution will be included in the next release! 🎉

### After Your PR is Merged

- Delete your branch
- Update your local repository
- Celebrate! 🥳

```bash
git checkout main
git pull upstream main
git branch -d feature/your-feature-name
```

---

## 🌍 Community

### Getting Help

[//]: # (- 💬 **Discord Community:** [discord.gg/revoicechat]&#40;https://discord.gg/revoicechat&#41;)
- 📖 **Contributing Guide:** [CONTRIBUTING.md](CONTRIBUTING.md)
- 🐛 **Report Issues:** [GitHub Issues](https://github.com/revoicechat/revoicechat/issues)

[//]: # (- 📧 **Contact:** hello@revoicechat.org)

### Recognition

Contributors are recognized in:
- Release notes

---

## ❤️ Thank You!

Your contributions make RevoiceChat better for everyone. We appreciate your time and effort!

**Happy coding!** 🚀