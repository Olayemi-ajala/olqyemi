# CLAUDE.md - AI Assistant Guide for olqyemi Repository

**Last Updated:** 2026-02-02
**Repository:** olqyemi
**Owner:** Olayemi-ajala
**Purpose:** Personal technology learning project

---

## Table of Contents

1. [Repository Overview](#repository-overview)
2. [Current State](#current-state)
3. [Technology Stack](#technology-stack)
4. [Codebase Structure](#codebase-structure)
5. [Development Workflows](#development-workflows)
6. [Git Conventions](#git-conventions)
7. [Code Conventions](#code-conventions)
8. [Testing Strategy](#testing-strategy)
9. [Documentation Standards](#documentation-standards)
10. [AI Assistant Guidelines](#ai-assistant-guidelines)
11. [Common Tasks](#common-tasks)
12. [Future Roadmap](#future-roadmap)

---

## Repository Overview

### Purpose
This repository serves as a learning environment for technology education and skill development. The owner (Olayemi-ajala) is actively learning tech, and this repository will evolve as new concepts, projects, and skills are acquired.

### Key Characteristics
- **Learning-focused:** Code and projects may be experimental or educational in nature
- **Iterative:** Expect frequent updates as new concepts are learned
- **Diverse:** May contain multiple small projects or exercises across different technologies
- **Documentation-heavy:** Emphasis on explaining "why" and "how" for learning purposes

---

## Current State

### Repository Status: **INITIALIZED**

As of 2026-02-02, this is a newly initialized repository with minimal content:

**Files Present:**
- `README.md` - Basic project introduction
- `CLAUDE.md` - This documentation file

**Git Status:**
- Current branch: `claude/add-claude-documentation-msHBd`
- Main branch: `main` (or default branch)
- Clean working tree
- Remote origin configured

**What's NOT Present (yet):**
- No source code files
- No dependency management files
- No build configuration
- No test suite
- No CI/CD pipeline
- No .gitignore file

### Next Steps for Development
1. Define primary technology stack (based on learning goals)
2. Set up project structure
3. Add appropriate .gitignore for chosen technologies
4. Configure development environment
5. Begin first project/exercise

---

## Technology Stack

### Current Technologies: **TO BE DETERMINED**

This section will be updated as technologies are chosen. Common stacks for learning include:

#### Potential Technologies (Update as Selected):
- **Frontend:** JavaScript/TypeScript, React, Vue, HTML/CSS
- **Backend:** Node.js, Python (Django/Flask), Java (Spring Boot)
- **Database:** PostgreSQL, MongoDB, SQLite
- **DevOps:** Docker, Git, GitHub Actions
- **Languages:** JavaScript, Python, Java, Go, Rust (TBD)

#### Dependencies
**Package Manager:** (TBD - npm, pip, maven, cargo, etc.)

When a technology is selected, update this section with:
- Version requirements
- Key dependencies
- Development tools
- Build tools

---

## Codebase Structure

### Recommended Directory Structure

Once development begins, organize code using a clear, logical structure. Here's a template:

```
olqyemi/
├── README.md                 # Project overview
├── CLAUDE.md                 # This file - AI assistant guide
├── .gitignore               # Git ignore patterns
├── LICENSE                  # Project license (if applicable)
│
├── docs/                    # Documentation
│   ├── learning-notes/      # Personal learning notes
│   ├── guides/              # How-to guides
│   └── references/          # Reference materials
│
├── projects/                # Individual learning projects
│   ├── project-1/
│   ├── project-2/
│   └── ...
│
├── exercises/               # Coding exercises and practice
│   ├── algorithms/
│   ├── data-structures/
│   └── ...
│
├── src/                     # Main source code (if single project)
│   ├── main/
│   └── test/
│
└── scripts/                 # Utility scripts
    ├── setup.sh
    └── ...
```

### File Naming Conventions

**General Rules:**
- Use lowercase with hyphens for directories: `my-project/`
- Use kebab-case or camelCase for files (be consistent within project)
- Use descriptive names: `user-authentication.js` not `ua.js`
- Test files: `*.test.js`, `*.spec.js`, or `test_*.py` depending on tech stack

---

## Development Workflows

### Setting Up Development Environment

```bash
# Clone repository
git clone [repository-url]
cd olqyemi

# Create feature branch
git checkout -b feature/your-feature-name

# Install dependencies (when package manager is set up)
# npm install
# pip install -r requirements.txt
# etc.

# Run development server (TBD based on project)
# npm run dev
# python manage.py runserver
# etc.
```

### Build Process

**Status:** Not yet configured

When build tools are added, document:
- Build commands
- Build outputs
- Build configurations
- Environment variables needed

### Deployment

**Status:** Not applicable yet

Future deployment strategies will be documented here.

---

## Git Conventions

### Branch Naming

**Convention:** Use descriptive branch names with prefixes

```
feature/add-user-authentication
bugfix/fix-login-error
docs/update-readme
refactor/restructure-components
claude/[task-description]-[session-id]  # For AI assistant work
```

**AI Assistant Branches:**
- Claude Code creates branches with pattern: `claude/*-[sessionId]`
- These branches are for AI-driven development work
- Always push to the designated claude/* branch for the session

### Commit Messages

**Format:** Use conventional commits style

```
<type>(<scope>): <subject>

<body>

<footer>
```

**Types:**
- `feat:` New feature
- `fix:` Bug fix
- `docs:` Documentation changes
- `style:` Code style changes (formatting, no logic change)
- `refactor:` Code refactoring
- `test:` Adding or updating tests
- `chore:` Maintenance tasks

**Examples:**
```
feat(auth): add user login functionality

Implement JWT-based authentication with login endpoint.
Includes password hashing and token generation.

https://claude.ai/code/session_xxxxx
```

```
docs: update CLAUDE.md with git conventions

Add detailed git workflow and branch naming conventions
for better collaboration and AI assistant guidance.
```

### Commit Best Practices

1. **Make atomic commits:** Each commit should represent one logical change
2. **Write clear messages:** Explain what and why, not how
3. **Commit often:** Small, frequent commits are better than large ones
4. **Don't commit secrets:** Never commit API keys, passwords, or sensitive data
5. **Use .gitignore:** Prevent committing build artifacts, dependencies, or local configs

### Pull Request Process

1. Create feature branch from main
2. Make changes and commit
3. Push branch to remote
4. Create Pull Request with:
   - Clear title and description
   - Summary of changes
   - Test plan
   - Link to related issues (if any)
5. Address review feedback
6. Merge when approved

---

## Code Conventions

### General Principles

1. **Clarity over cleverness:** Write code that's easy to understand
2. **Consistency:** Follow established patterns in the codebase
3. **DRY (Don't Repeat Yourself):** Extract common logic into reusable functions
4. **KISS (Keep It Simple):** Avoid unnecessary complexity
5. **Comments:** Explain "why" not "what" (code should be self-documenting)

### Language-Specific Conventions

**JavaScript/TypeScript:**
- Use `const` by default, `let` when reassignment needed, avoid `var`
- Use arrow functions for callbacks
- Use template literals for string interpolation
- Prefer async/await over promise chains
- Use meaningful variable names (avoid single letters except in loops)

**Python:**
- Follow PEP 8 style guide
- Use snake_case for functions and variables
- Use PascalCase for classes
- Use type hints where appropriate
- Maximum line length: 88 characters (Black formatter default)

**General:**
- Indent with 2 or 4 spaces (be consistent, configure .editorconfig)
- Use meaningful variable and function names
- Keep functions small and focused (single responsibility)
- Avoid deep nesting (max 3-4 levels)

### Code Organization

- Group related functionality together
- Separate concerns (UI, business logic, data access)
- Use meaningful directory and file names
- One component/class per file (in most cases)
- Order imports: standard library, third-party, local

---

## Testing Strategy

### Testing Philosophy

**Current Status:** No tests yet

**Future Approach:**
- Write tests for new features
- Aim for meaningful test coverage (not just high percentage)
- Test behavior, not implementation details
- Use descriptive test names

### Testing Levels

1. **Unit Tests:** Test individual functions/components in isolation
2. **Integration Tests:** Test how components work together
3. **End-to-End Tests:** Test complete user workflows

### Test Structure

```javascript
// Example: Jest/Mocha style
describe('ComponentName', () => {
  describe('functionName', () => {
    it('should do something specific', () => {
      // Arrange
      const input = 'test';

      // Act
      const result = functionName(input);

      // Assert
      expect(result).toBe('expected');
    });
  });
});
```

### Running Tests

**TBD based on testing framework chosen**

```bash
# npm test
# pytest
# go test
# cargo test
```

---

## Documentation Standards

### Code Documentation

**When to Document:**
- Public APIs and interfaces
- Complex algorithms or logic
- Non-obvious design decisions
- Setup and configuration steps

**When NOT to Document:**
- Obvious code that speaks for itself
- Implementation details (prefer clear code)

**Good Comment:**
```javascript
// Use exponential backoff to avoid overwhelming the API
// during high traffic periods
await retryWithBackoff(apiCall, { maxRetries: 3 });
```

**Bad Comment:**
```javascript
// Increment counter by 1
counter++;
```

### Project Documentation

**Essential Files:**
1. **README.md** - Project overview, setup instructions, basic usage
2. **CLAUDE.md** - This file, for AI assistant guidance
3. **CONTRIBUTING.md** - Contribution guidelines (if open source)
4. **CHANGELOG.md** - Version history and changes
5. **docs/** - Detailed documentation, guides, tutorials

### Learning Documentation

Since this is a learning repository:
- Document what you learned
- Explain concepts in your own words
- Link to resources that helped
- Include examples and exercises

---

## AI Assistant Guidelines

### General Principles for AI Assistants (Claude Code)

1. **Understand before modifying:** Always read existing code before making changes
2. **Follow repository conventions:** Adhere to styles and patterns in this document
3. **Be educational:** Since this is a learning repo, explain decisions and suggest best practices
4. **Ask when unclear:** If requirements are ambiguous, ask for clarification
5. **Think incrementally:** Break large tasks into smaller, manageable steps
6. **Test your changes:** Verify code works before committing
7. **Document as you go:** Update this file when patterns or conventions change

### Specific Guidelines

#### When Adding New Features
1. Check if similar functionality exists
2. Follow existing architectural patterns
3. Write tests for new code
4. Update documentation
5. Use clear, descriptive variable/function names
6. Keep changes focused and atomic

#### When Fixing Bugs
1. Understand the root cause before fixing
2. Add tests to prevent regression
3. Document the fix in commit message
4. Consider if similar bugs exist elsewhere

#### When Refactoring
1. Don't change behavior
2. Make one type of change at a time
3. Ensure tests pass after refactoring
4. Improve code clarity and structure

#### When Learning is the Goal
- Explain concepts clearly
- Provide examples and alternatives
- Suggest resources for deeper learning
- Encourage experimentation
- Be patient with mistakes

### AI Assistant Workflow

```
1. Receive task → Understand requirements
2. Explore codebase → Read relevant files
3. Plan approach → Break into steps, use TodoWrite tool
4. Implement → Make changes incrementally
5. Test → Verify functionality
6. Document → Update code comments and docs
7. Commit → Use conventional commit format
8. Push → To designated branch (claude/*)
```

### Tools Usage

- **Read:** Always read files before editing
- **Edit:** For modifying existing files (preferred over Write)
- **Write:** For creating new files only
- **Bash:** For git operations, running tests, building
- **Grep/Glob:** For searching codebase
- **Task:** For complex multi-step tasks
- **TodoWrite:** For tracking tasks and planning

### Prohibited Actions

1. **Never commit secrets:** API keys, passwords, tokens
2. **Never force push:** Unless explicitly requested
3. **Never delete important files:** Without confirmation
4. **Never skip tests:** If they exist and should pass
5. **Never ignore errors:** Address or report them
6. **Never over-engineer:** Keep solutions simple and focused

---

## Common Tasks

### Creating a New Project

```bash
# Create project directory
mkdir projects/my-new-project
cd projects/my-new-project

# Initialize based on technology
# npm init -y
# python -m venv venv
# cargo init
# etc.

# Create basic structure
mkdir src tests docs
touch README.md

# Add .gitignore
# Copy from https://github.com/github/gitignore

# Make initial commit
git add .
git commit -m "feat: initialize my-new-project"
```

### Adding Dependencies

**JavaScript:**
```bash
npm install package-name
npm install --save-dev dev-package-name
```

**Python:**
```bash
pip install package-name
pip freeze > requirements.txt
```

### Running Code

**TBD based on project type**

Document specific run commands when projects are created.

### Updating Documentation

When making changes:
1. Update relevant README.md sections
2. Update CLAUDE.md if conventions change
3. Add inline comments for complex logic
4. Update CHANGELOG.md for version releases

---

## Future Roadmap

### Immediate Next Steps

1. **Set up .gitignore** - Choose technologies and add appropriate ignore patterns
2. **Choose first project** - Decide what to build/learn first
3. **Set up development environment** - Install necessary tools
4. **Create project structure** - Set up directories and files
5. **Write first code** - Start learning and building

### Short-term Goals

- [ ] Define primary technology stack
- [ ] Complete first tutorial/project
- [ ] Set up testing framework
- [ ] Add CI/CD pipeline
- [ ] Build 3-5 small projects

### Long-term Vision

- Build portfolio of diverse projects
- Master chosen technology stack
- Contribute to open source
- Build deployable applications
- Document learning journey

---

## Appendix

### Useful Resources

**General Learning:**
- [freeCodeCamp](https://www.freecodecamp.org/)
- [The Odin Project](https://www.theodinproject.com/)
- [MDN Web Docs](https://developer.mozilla.org/)
- [GitHub Learning Lab](https://lab.github.com/)

**Git:**
- [Pro Git Book](https://git-scm.com/book/en/v2)
- [Conventional Commits](https://www.conventionalcommits.org/)

**Best Practices:**
- [Clean Code by Robert C. Martin](https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882)
- [The Pragmatic Programmer](https://pragprog.com/titles/tpp20/)

### Contact & Support

**Repository Owner:** Olayemi-ajala
**Issues:** Use GitHub Issues for tracking bugs and features
**Questions:** Document questions and answers in docs/learning-notes/

---

## Version History

| Version | Date       | Changes                                    |
|---------|------------|--------------------------------------------|
| 1.0.0   | 2026-02-02 | Initial CLAUDE.md creation with comprehensive guide |

---

**Note to AI Assistants:** This document should be updated regularly as the repository evolves. When making significant changes to the codebase structure, conventions, or workflows, please update the relevant sections in this file to keep it accurate and useful.
