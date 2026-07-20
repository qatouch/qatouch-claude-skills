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
from the `skills/` folder without cloning everything. All `.skill` files live
directly inside the `skills/` directory.

You can also download a specific skill archive with a direct URL:

```bash
# Example: download a specific skill archive
curl -L -o jira-qatouch-case-generator.skill \
  https://raw.githubusercontent.com/qatouch/qatouch-claude-skills/main/skills/jira-qatouch-case-generator.skill
```

Adjust the URL to match the skill and branch you need.

## Importing a Skill into Claude Desktop

Each installable Claude Skill is a `.skill` file located directly inside the
`skills/` folder. To install a skill:

1. Browse to the `skills/` folder in this repository.
2. Download the desired `.skill` file.
3. Open Claude Desktop.
4. Go to **Settings → Customize → Skills**.
5. Click **Add**.
6. Select **Upload a Skill**.
7. Choose the downloaded `.skill` file.
8. Import the `.skill` file into your Claude environment.
9. Invoke the skill using `/skill-name` whenever you need it.

## Updating Skills

Each installable Claude Skill is a `.skill` file located directly inside the
`skills/` folder. To update a skill to a newer version:

1. Browse to the `skills/` folder in this repository.
2. Download the latest `.skill` file for the skill.
3. Open Claude Desktop.
4. Go to **Settings → Customize → Skills**.
5. Upload the new `.skill` file, replacing the previous version.

We recommend tracking the version number recorded in the repository
`CHANGELOG.md` and `skills/README.md` so you know when an update is available.
