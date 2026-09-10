# QA Touch Claude Skills

A collection of open-source [Claude Skills](https://claude.com) for QA
engineers, testers, and engineering teams. These skills accelerate
software testing workflows by connecting Claude to the tools QA teams already
use, such as Jira, Playwright, and QA Touch.

## What Are Claude Skills?

Claude Skills are packaged, reusable sets of instructions that extend what
Claude can do for a specific task. A skill bundles domain knowledge, workflows,
and best practices into a single file that can be imported into Claude. Once
imported, Claude can apply the skill to perform specialized work, such as
generating test cases or analyzing requirements, without the user having to
write detailed prompts from scratch.

## Why QA Touch Publishes These Skills

QA Touch builds tooling for modern QA and test management. Many testing tasks
are repetitive, time-consuming, or require specific domain knowledge. By
publishing Claude Skills, QA Touch aims to:

- Reduce the manual effort involved in test design and test management.
- Help teams improve test coverage with consistent, repeatable workflows.
- Make AI-assisted testing accessible to QA engineers of all experience levels.
- Integrate AI workflows directly with the tools teams already use.

## Repository Layout

```
.
├── README.md              # This file
├── LICENSE                # MIT License
├── CHANGELOG.md           # Release history
├── CONTRIBUTING.md        # Contribution guidelines
├── CODE_OF_CONDUCT.md     # Community standards
├── SECURITY.md            # Vulnerability reporting
├── .gitignore
├── .gitattributes
├── .github/               # Issue templates, PR template, CI workflows
├── docs/                  # Extended documentation
└── skills/               # All downloadable .skill files
```

## Available Skills

| Skill | File | Description | Status |
|------|------|-------------|--------|
| Jira QA Touch Case Generator | [`jira-qatouch-case-generator.skill`](skills/jira-qatouch-case-generator.skill) | Generates QA Touch import-ready manual test cases directly from Jira Stories | Available |
| Capture Browser Automatically Action | [`jira-qatouch-case-generator.skill`](skills/qatouch-capture-testcases.skill) | Automatically Capture Browser Actions generate Test Case Steps | Available |

## Installation

Each installable Claude Skill is a `.skill` file located directly inside the
`skills/` folder. See [docs/installation.md](docs/installation.md) for detailed
instructions.

In short:

1. Browse to the `skills/` folder and download the desired `.skill` file.
2. Open Claude Desktop and go to **Settings → Customize → Skills**.
3. Click **Add**, select **Upload a Skill**, and choose the downloaded file.
4. Invoke the skill using `/skill-name` whenever you need it.

## Usage

See [docs/usage.md](docs/usage.md) for guidance on choosing the right skill,
best practices, and working with connectors and QA Touch.

## Repository Structure

- `skills/` — The central location containing all downloadable `.skill` files.
- `docs/` — Extended guides covering installation, usage, and frequently asked
  questions.
- `.github/` — Community templates and continuous integration workflows.

## Contributing

Contributions are welcome. Please read
[CONTRIBUTING.md](CONTRIBUTING.md) before opening a pull request. It covers
documentation standards, naming conventions, the pull request process, and a
testing checklist for publishing skills.

## License

This repository is licensed under the [MIT License](LICENSE).
