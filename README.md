# Claude Code Development Environment

A starter template for configuring projects to work effectively with [Claude Code](https://docs.anthropic.com/en/docs/claude-code), Anthropic's official CLI tool for AI-assisted software development.

## Overview

This repository provides configuration templates that help Claude Code understand your project structure, coding conventions, and workflows. By customizing these files for your project, you enable Claude Code to provide more accurate and context-aware assistance.

## Contents

| File | Purpose |
|------|---------|
| `CLAUDE.md` | Project-specific instructions and context for Claude Code |
| `AGENTS.md` | Configuration for custom AI agents (optional) |
| `.claude/settings.local.json` | Local Claude Code permissions and settings |

## Getting Started

### 1. Copy the Template Files

Copy the template files to your project's root directory:

```bash
# Copy the main configuration file
cp CLAUDE.md /path/to/your/project/

# Optionally copy agents configuration
cp AGENTS.md /path/to/your/project/

# Copy local settings (optional)
mkdir -p /path/to/your/project/.claude
cp .claude/settings.local.json /path/to/your/project/.claude/
```

### 2. Customize CLAUDE.md

Edit `CLAUDE.md` to match your project:

1. **Repository Overview** - Add your project name, purpose, status, and tech stack
2. **Project Structure** - Document your directory layout
3. **Quick Start** - Add installation and build commands
4. **Architecture Patterns** - Describe your project's architecture
5. **Development Workflows** - Document common tasks and conventions
6. **Configuration** - List environment variables and config files
7. **Testing** - Add test commands and conventions
8. **Git Workflow** - Define your branching and commit conventions

### 3. Configure Permissions (Optional)

Edit `.claude/settings.local.json` to control which tools Claude Code can use:

```json
{
  "permissions": {
    "allow": [
      "tool_name_1",
      "tool_name_2"
    ]
  }
}
```

## Template Sections

### CLAUDE.md Structure

The `CLAUDE.md` template includes these sections:

- **Repository Overview** - Project purpose, status, and technology stack
- **Project Structure** - Directory layout with descriptions
- **Quick Start** - Installation, build, test, and lint commands
- **Architecture Patterns** - Core, shared, and feature module patterns
- **Key Technologies** - Components and utilities used
- **Development Workflows** - Common development tasks
- **Configuration** - Environment and config files
- **Deployment** - Docker and server deployment instructions
- **Testing** - Unit test conventions and commands
- **Best Practices** - Code style and design guidelines
- **Version Control Guidelines** - Commit conventions and Git workflow
- **Troubleshooting** - Common issues and solutions

### Commit Convention

The template enforces these commit prefixes:

| Prefix | Usage |
|--------|-------|
| `ai-tooling` | AI agents, automation, workflows |
| `feat` | New features |
| `fix` | Bug fixes |
| `docs` | Documentation |
| `style` | Formatting changes |
| `refactor` | Code restructuring |
| `test` | Adding tests |
| `chore` | Maintenance tasks |

## Best Practices

1. **Keep CLAUDE.md Updated** - Update the file as your project evolves
2. **Be Specific** - The more detail you provide, the better Claude Code can assist
3. **Document Conventions** - Include coding standards and patterns your team follows
4. **Add Examples** - Include code examples for common patterns
5. **List Dependencies** - Document key dependencies and their purposes

## Resources

- [Claude Code Documentation](https://docs.anthropic.com/en/docs/claude-code)
- [Claude Code GitHub](https://github.com/anthropics/claude-code)
- [AGENTS.md](https://agents.md)

## License

This template is provided as-is for use in your projects. Customize freely to fit your needs.
