# Installation

This guide explains how to obtain and install QA Touch Claude Skills. It is kept
generic so it remains valid even as the Claude user interface evolves.

## Cloning the Repository

You can clone the entire repository to access all published skills and
documentation:

```bash
git clone https://github.com/qatouch/qatouch-claude-skills.git
cd qatouch-claude-skills
```

After cloning, all installable skills are available directly inside the
`skills/` directory as `.skill` files.

## Downloading Individual `.skill` Files

If you only need a single skill, you can download its `.skill` file directly
from the repository without cloning everything. All `.skill` files live directly
inside the `skills/` directory.

1. Navigate to the `skills` folder in this repository.
2. Download the desired `.skill` file (for example
   `jira-qatouch-case-generator.skill`).
3. Import the downloaded file into Claude Desktop.

You can also download a specific skill archive with a direct URL:

```bash
# Example: download a specific skill archive
curl -L -o jira-qatouch-case-generator.skill \
  https://raw.githubusercontent.com/qatouch/qatouch-claude-skills/main/skills/jira-qatouch-case-generator.skill
```

Adjust the URL to match the skill and branch you need.

## Importing Skills into Claude

Claude Skills are imported as `.skill` archives. The import process generally
follows these steps:

1. Open your Claude environment or client.
2. Locate the option to manage or import skills (often found in the skills or
   settings area).
3. Select the `.skill` file you downloaded or cloned.
4. Confirm the import. The skill becomes available by its name.

Because the exact menu labels may change between Claude releases, refer to the
official Claude documentation for the most current import instructions. The
`.skill` file format remains stable regardless of UI changes.

## Updating Skills

To update a skill to a newer version:

1. Re-download the latest `.skill` file from this repository.
2. Import the new version into Claude, replacing the previous one.

We recommend tracking the version number recorded in the repository
`CHANGELOG.md` and `skills/README.md` so you know when an update is available.
