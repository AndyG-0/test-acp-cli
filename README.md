# Test ACP CLI Repository

This is a test repository for validating agent, skill, instruction, and prompt discovery in both the root directory and `.github` folder locations.

## Repository Structure

```
├── agents/                          # Root-level agents
│   └── sample-agent.agent.md
├── prompts/                         # Root-level prompts
│   └── sample-prompt.prompt.md
├── instructions/                    # Root-level instructions
│   └── sample-instructions.instructions.md
├── skills/                          # Root-level skills
│   ├── README.md
│   └── sample-skill/
│       └── skill.md
├── .github/                         # GitHub folder for testing
│   ├── agents/
│   │   └── github-agent.agent.md
│   ├── prompts/
│   │   └── github-prompt.prompt.md
│   ├── instructions/
│   │   └── github-instructions.instructions.md
│   └── skills/
│       ├── README.md
│       └── github-skill/
│           └── skill.md
└── README.md
```

## File Naming Conventions

- **Agents**: `*.agent.md` (e.g., `sample-agent.agent.md`)
- **Prompts**: `*.prompt.md` (e.g., `sample-prompt.prompt.md`)
- **Instructions**: `*.instructions.md` (e.g., `sample-instructions.instructions.md`)
- **Skills**: Folders containing `skill.md` and supporting files

## File Structure

All files include YAML frontmatter with metadata:

```yaml
---
name: Display Name
description: Brief description
author: Author Name
version: 1.0.0
---
```

### Additional Properties

- **Instructions** files include `applyTo` to specify file patterns
- **Skills** are organized as folders containing a `skill.md` file

## Testing

This repository is designed to:

1. Test agent discovery in both root and `.github` folders
2. Validate prompt discovery mechanisms
3. Verify instruction file pattern matching
4. Check skill folder detection and organization

### Sample Files Included

- `agents/sample-agent.agent.md` - Root-level agent
- `.github/agents/github-agent.agent.md` - GitHub folder agent
- `prompts/sample-prompt.prompt.md` - Root-level prompt
- `.github/prompts/github-prompt.prompt.md` - GitHub folder prompt
- `instructions/sample-instructions.instructions.md` - Root-level instructions
- `.github/instructions/github-instructions.instructions.md` - GitHub folder instructions
- `skills/sample-skill/skill.md` - Root-level skill
- `.github/skills/github-skill/skill.md` - GitHub folder skill

## Usage

Use this repository to test various ACP (Awesome Copilot) tools and configurations that need to discover and load agents, prompts, instructions, and skills from both standard and alternate folder locations.

## Notes

- All files are minimal/sample implementations suitable for testing
- Complete functionality is not required for testing purposes
- Both root and `.github` folder locations are populated for comprehensive testing
