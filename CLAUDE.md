# CLAUDE.md - Project Context

This file provides context and guidelines for Claude when working with this project.

## Project Overview

This is a sample Claude plugin that demonstrates best practices for plugin development. It serves as a boilerplate template for creating new Claude plugins.

## Directory Structure

```
.
├── .claude-plugin/       # Plugin metadata (required)
│   └── plugin.json       # Plugin manifest
├── commands/             # User-invoked slash commands
│   ├── hello.md          # Example greeting command
│   └── help.md           # Help documentation command
├── agents/               # Specialized AI agents
│   ├── code-reviewer.md  # Code review specialist
│   └── test-writer.md    # Test writing specialist
├── skills/               # Model-invoked capabilities
│   └── api-integration/
│       └── SKILL.md      # API integration skill
├── hooks/                # Lifecycle hooks
│   └── hooks.json        # Hook configurations
├── .mcp.json             # MCP server definitions
├── CLAUDE.md             # This file - project context
├── README.md             # User documentation
└── LICENSE               # MIT License
```

## Development Guidelines

### Adding New Commands

1. Create a new `.md` file in the `commands/` directory
2. Include usage, description, arguments, and examples
3. Provide clear instructions for the command behavior

### Adding New Agents

1. Create a new `.md` file in the `agents/` directory
2. Define the agent's role, capabilities, and guidelines
3. Specify the output format and context requirements

### Adding New Skills

1. Create a new directory in `skills/`
2. Add a `SKILL.md` file with skill description and capabilities
3. Include when the skill should be invoked and best practices

## Conventions

- Use semantic versioning for plugin versions
- Keep documentation up to date with changes
- Follow the existing file structure patterns
- Test changes before publishing

## Common Tasks

- **Update plugin metadata**: Edit `.claude-plugin/plugin.json`
- **Add a command**: Create new `.md` file in `commands/`
- **Add an agent**: Create new `.md` file in `agents/`
- **Configure hooks**: Modify `hooks/hooks.json`
