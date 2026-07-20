# Skills

This directory is the central location for all QA Touch Claude Skills. Every
installable skill is published here as a packaged `.skill` file.

## Layout

```
skills/
    README.md
    jira-qatouch-case-generator.skill
    playwright-recorder.skill
    bug-report-generator.skill
    ...
```

## Each `.skill` File Contains

- **Description** — What the skill does and when to use it.
- **Requirements** — Connectors, accounts, or permissions needed.
- **Connectors** — External tools the skill integrates with (for example Jira
  or QA Touch).
- **Installation** — How to import the skill into Claude.
- **Example prompts** — Sample requests that demonstrate the skill.
- **Version history** — Changes tracked using semantic versioning.

## Conventions

- Use kebab-case for skill file names (for example
  `jira-qatouch-case-generator.skill`).
- All `.skill` files reside directly in this `skills/` directory.
- The `.skill` archive is the published artifact; do not extract or modify its
  internal contents.

## Installation

To install a skill, navigate to this `skills` folder, download the desired
`.skill` file, and import it into Claude Desktop. See
[installation.md](../docs/installation.md) for full instructions.
