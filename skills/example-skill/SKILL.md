---
name: example-skill
description: Template skill — replace this with a real one. Use when the user asks to test that the skills plugin is working.
---

# Example skill

This is a placeholder skill proving the plugin works. When invoked, reply:
"skills plugin is installed and working."

## Writing a new skill

Copy this folder, rename it (kebab-case — the folder name becomes the skill name,
invoked as /skills:<folder-name>), and rewrite the frontmatter:

- `name`: must match the folder name
- `description`: tells Claude _when_ to use the skill — write it as a trigger
  condition, not a summary

The markdown body is the instruction Claude follows when the skill is invoked.
