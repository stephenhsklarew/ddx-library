# DDx Library

This repository contains the DDx (Document-Driven Development eXperience) library of templates, patterns, prompts, and configurations for AI-assisted development.

## Installation

### Claude Code Plugin (Recommended)

Install directly as a Claude Code plugin:

```bash
/plugin install https://github.com/easel/ddx-library
```

This gives you:
- **Slash commands**: `/ddx:prd`, `/ddx:code-review`, `/ddx:commit-hooks`, `/ddx:github-actions`, `/ddx:docs`, `/ddx:gitignore`, `/ddx:create-workflow`
- **HELIX skill**: Auto-invoked TDD workflow guidance during development
- **Agents**: Systems architect, TDD test engineer, strict code reviewer

### DDx CLI

Alternatively, use the [DDx CLI tool](https://github.com/easel/ddx) for git subtree-based synchronization:

```bash
# Install DDx CLI
curl -fsSL https://raw.githubusercontent.com/easel/ddx/main/install.sh | bash

# Initialize in your project
ddx init
```

## Contents

- **commands/** - Claude Code slash commands
- **skills/** - Auto-invoked Claude Code skills (HELIX workflow)
- **agents/** - Specialized Claude Code agents
- **prompts/** - AI prompts and instructions for various development tasks
- **personas/** - AI personality definitions for consistent interactions
- **mcp-servers/** - Model Context Protocol server configurations
- **workflows/** - Complete development methodologies (HELIX, etc.)
- **environments/** - Development environment configurations
- **tools/** - Development tool integrations and scripts
- **templates/** - Project templates and boilerplates
- **patterns/** - Reusable code patterns and solutions

## Contributing

We welcome contributions! To contribute improvements:

1. **Via DDx CLI**: Make changes to your local `.ddx/` directory and run `ddx contribute`
2. **Via GitHub**: Fork this repository, make changes, and submit a pull request
3. **Via git subtree**: Make changes locally and use `git subtree push` to contribute back

## License

This library is open source software licensed under the MIT License.

## Related Projects

- [DDx CLI](https://github.com/easel/ddx) - The command-line tool for using this library
- [HELIX Workflow](./workflows/helix/) - Six-phase AI-assisted development methodology