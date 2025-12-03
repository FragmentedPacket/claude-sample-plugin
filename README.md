# Claude Sample Plugin

A boilerplate Claude plugin demonstrating best practices and folder structure for plugin development.

## 🚀 Quick Start

1. Clone this repository
2. Customize the `plugin.json` with your plugin details
3. Add your commands, agents, and skills
4. Install the plugin in Claude

## 📁 Project Structure

```
.
├── .claude-plugin/         # Required: Plugin metadata
│   └── plugin.json         # Required: Plugin manifest
├── commands/               # Optional: User-invoked slash commands
│   ├── hello.md            # Example greeting command
│   └── help.md             # Help documentation command
├── agents/                 # Optional: Specialized AI agents
│   ├── code-reviewer.md    # Code review specialist
│   └── test-writer.md      # Test writing specialist
├── skills/                 # Optional: Model-invoked capabilities
│   └── api-integration/
│       └── SKILL.md        # API integration skill
├── hooks/                  # Optional: Lifecycle hooks
│   └── hooks.json          # Hook configurations
├── .mcp.json               # Optional: MCP server definitions
├── CLAUDE.md               # Recommended: Project context for Claude
├── README.md               # Recommended: This documentation
└── LICENSE                 # Recommended: MIT License
```

## 📋 Components

### Plugin Manifest (`.claude-plugin/plugin.json`)

The only required file. Contains plugin metadata:

```json
{
  "name": "sample-plugin",
  "version": "1.0.0",
  "description": "A sample Claude plugin demonstrating best practices and folder structure",
  "keywords": ["sample", "boilerplate", "template", "claude-code"],
  "strict": true
}
```

### Commands (`commands/`)

Slash commands that users can invoke directly. Each command is a Markdown file with:
- Usage instructions
- Description
- Arguments
- Examples
- Implementation instructions

### Agents (`agents/`)

Specialized AI agents with defined roles and capabilities. Each agent is a Markdown file containing:
- Role definition
- Capabilities list
- Guidelines for behavior
- Output format specifications

### Skills (`skills/`)

Model-invoked capabilities that Claude can use automatically. Each skill has a `SKILL.md` file with:
- Description
- Capabilities
- When to use
- Best practices

### Hooks (`hooks/`)

Lifecycle hooks for pre/post actions on commits, pushes, and error handling. Configured in `hooks.json`.

### MCP Configuration (`.mcp.json`)

Optional Model Context Protocol server definitions for extended functionality.

### Project Context (`CLAUDE.md`)

Project-specific context and guidelines that help Claude understand your codebase.

## 🛠️ Customization

1. **Edit `plugin.json`**: Update name, version, description, and keywords
2. **Add Commands**: Create new `.md` files in `commands/`
3. **Add Agents**: Create new `.md` files in `agents/`
4. **Add Skills**: Create new directories in `skills/` with `SKILL.md` files
5. **Configure Hooks**: Modify `hooks/hooks.json` for lifecycle events
6. **Update Context**: Edit `CLAUDE.md` with your project specifics

## 📖 Best Practices

- Use semantic versioning for your plugin version
- Enable `strict` mode for better error handling
- Keep documentation up to date
- Use descriptive names for commands, agents, and skills
- Follow consistent formatting in Markdown files
- Test your plugin thoroughly before publishing

## 📄 License

MIT License - see [LICENSE](LICENSE) for details