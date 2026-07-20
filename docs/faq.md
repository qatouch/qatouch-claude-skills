# FAQ

## What is a Claude Skill?

A Claude Skill is a packaged set of instructions that extends what Claude can do
for a specific task. Skills bundle domain knowledge and workflows into a single
importable file, letting Claude perform specialized work without you having to
write detailed prompts from scratch.

## Do I need QA Touch?

Not always. Some skills are general purpose, while others produce artifacts
designed for QA Touch or depend on connectors such as Jira. Each skill's
`README.md` lists its requirements. If a skill targets QA Touch, you will need a
QA Touch account to use the generated output.

## Can I modify skills?

The packaged `.skill` files are published artifacts. You are free to use them as
provided. If you want to propose changes, fork the repository and open a pull
request following the guidelines in `CONTRIBUTING.md`.

## How do I update skills?

Re-download the latest `.skill` file from this repository and import it,
replacing the previous version. Track versions via the repository `CHANGELOG.md`
and `skills/README.md`. See [installation.md](installation.md) for
details.

## How do I report bugs?

Open a bug report using the template in `.github/ISSUE_TEMPLATE/bug_report.md`,
or report security issues privately as described in `SECURITY.md`.

## Will more skills be added?

Yes. QA Touch plans to publish additional skills over time covering automation,
bug reporting, requirement analysis, test generation, release management, and
more. Check the repository and the `skills/` folder for newly added `.skill`
files.
