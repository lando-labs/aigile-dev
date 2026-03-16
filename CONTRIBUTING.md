# Contributing to AIgile Dev

Thanks for your interest in contributing to AIgile Dev! This plugin brings AI-native agile workflows to Claude Code.

## Getting Started

1. Fork the repository
2. Clone your fork locally
3. Create a branch for your changes

## Project Structure

```
aigile-dev/
├── agents/           # Methodology-focused agents
├── skills/           # Workflow skills
│   ├── vibecoding-sprint/   # Sprint planning skill
│   └── research/            # Research deliverable skills
├── reference/        # Documentation and glossaries
├── .claude-plugin/   # Plugin manifest
├── CLAUDE.md         # Plugin instructions
└── LICENSE           # MIT license
```

## Types of Contributions

### Bug Reports

Open an issue with:
- Clear description of the bug
- Steps to reproduce
- Expected vs actual behavior
- Which agent or skill is affected

### Feature Requests

Open an issue with:
- Problem you're trying to solve
- Proposed solution
- Which agent or skill this relates to

### Pull Requests

1. **Agents**: Follow the Research → Build → Follow-up methodology
2. **Skills**: Include SKILL.md with clear triggers and outputs
3. **Documentation**: Keep it concise and actionable

## Code Style

### Agents

- Use YAML frontmatter with required fields (name, version, description, class, specialty)
- Include clear DO/DON'T/ESCALATE boundaries
- Add self-verification checklist
- Keep methodology-focused, not implementation-specific

### Skills

- Include frontmatter with name, description, and allowed-tools
- Document trigger phrases
- Provide output templates
- Keep tech-stack agnostic where possible

## Testing

Since this is a Claude Code plugin:
- Test agents by invoking them in Claude Code
- Test skills by using their trigger phrases
- Verify outputs match expected templates

## Commit Messages

Follow the convention:
```
[scope] type: description

Examples:
- [agent] feat: add qa-lead agent
- [skill] fix: correct sprint manifest template
- [docs] update: add glossary terms
```

## Questions?

Open an issue with the `question` label.

## License

By contributing, you agree that your contributions will be licensed under the MIT License.
