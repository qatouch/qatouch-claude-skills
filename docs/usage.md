# Usage

This guide explains how to get the most out of QA Touch Claude Skills. It is
kept generic so it stays relevant as the Claude user interface evolves.

## Choosing the Correct Skill

Each skill is designed for a specific QA task. Before starting, review the
skill's description to confirm it matches your goal. The
[main README](../README.md) includes a table of currently available skills, and
the `skills/` directory lists every downloadable `.skill` file.

When in doubt, select the skill whose stated purpose most closely matches the
outcome you want (for example generating test cases versus analyzing
requirements).

## Best Practices

- Read the skill's description before first use, including its requirements and
  example prompts.
- Provide clear, specific context when invoking a skill. The more relevant
  detail you supply, the better the result.
- Treat generated output as a starting point. Review and adapt test cases,
  reports, or analyses to your project's standards.
- Keep your source data (Jira stories, requirements, etc.) well structured so
  connectors can access what the skill needs.

## Keeping Skills Updated

Each installable Claude Skill is a `.skill` file located directly inside the
`skills/` folder. Skills improve over time. Check the repository `CHANGELOG.md`
and each skill's description for version changes, then re-import the latest
`.skill` file using the workflow in [installation.md](installation.md) when an
update is available. Invoke a skill using `/skill-name` whenever you need it.

## Using Skills with Connectors

Many skills rely on connectors to external tools such as Jira or QA Touch. A
connector gives Claude secure access to the data the skill needs. Before using a
connector-based skill:

- Ensure the relevant connector is configured in your Claude environment.
- Confirm you have the necessary permissions to read the source data.
- Verify the skill's description lists the connector it requires.

If a skill reports a connection issue, check that the connector is enabled and
that your account has access to the referenced project or resource.

## Using Skills with QA Touch

Skills that target QA Touch produce artifacts you can import directly into your
QA Touch workspace, such as CSV test case files. After a skill generates output:

1. Review the generated file for accuracy and coverage.
2. Import it into QA Touch using the standard import workflow for that artifact
   type.
3. Organize the imported items into the relevant project, module, or test suite.

Because import steps may vary by QA Touch release, consult QA Touch
documentation for the current import procedure.
