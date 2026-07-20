# Contributing to QA Touch Claude Skills

Thank you for your interest in contributing to the QA Touch Claude Skills repository.
This document describes the standards and processes we follow when accepting
contributions.

## Documentation Standards

- Write in clear, professional English aimed at developers and QA engineers.
- Keep documentation focused on usage and mechanics; avoid marketing language.
- Prefer examples over lengthy explanations.
- Update `README.md`, `CHANGELOG.md`, and the relevant `docs/` file whenever a
  skill is added or changed.
- Do not include secrets, API keys, or personal data in any documentation.

## Skill Naming Conventions

- Use lowercase, hyphen-separated names (kebab-case), for example
  `jira-qatouch-case-generator`.
- Names must be descriptive and reflect the primary purpose of the skill.
- Do not use spaces, underscores, or camelCase.
- Keep names reasonably short while remaining unambiguous.

## File Conventions

- Every installable skill is published as a `.skill` file directly inside the
  `skills/` directory.
- Name the file in kebab-case after the skill, for example
  `jira-qatouch-case-generator.skill`.
- Do not extract, modify, or duplicate the internal contents of a `.skill`
  archive. Treat the archive as the published artifact.

## Pull Request Process

1. Fork the repository and create a feature branch from `main`.
2. Add or update the skill and its documentation.
3. Update `README.md` to include the new skill in the available skills table.
4. Add a `CHANGELOG.md` entry describing your change.
5. Open a pull request with a clear title and description.
6. Ensure the Markdown lint workflow passes.
7. A maintainer will review, request changes if needed, and merge.

## Versioning Recommendations

- Version each skill independently using semantic versioning
  (MAJOR.MINOR.PATCH).
- Increment MAJOR for breaking changes, MINOR for new functionality, and PATCH
  for fixes.
- Record the skill version in its `README.md` and include it in the
  repository `CHANGELOG.md`.

## Testing Checklist Before Publishing a Skill

Before submitting a skill for review, verify:

- [ ] The skill loads correctly in the target Claude environment.
- [ ] All documented example prompts produce the expected output.
- [ ] Required connectors are clearly stated in the skill README.
- [ ] No secrets, credentials, or personal data are included.
- [ ] Documentation is accurate and free of placeholder or TODO text.
- [ ] The skill name and folder follow the naming conventions.
- [ ] The `README.md` and `CHANGELOG.md` are updated.
