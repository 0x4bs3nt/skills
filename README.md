# skills

Personal custom-written skills for agents, packaged as a Claude Code plugin
(`skills`) so they're available in every project.

## Structure

```text
.claude-plugin/
  plugin.json        # plugin manifest
  marketplace.json   # makes this repo installable as a marketplace
skills/
  <skill-name>/
    SKILL.md         # one folder per skill; folder name = skill name
```

## Install (once)

In any Claude Code session:

```text
/plugin marketplace add 0x4bs3nt/skills
/plugin install skills@4bs3nt-skills
```

Choose **user scope** when prompted so the skills apply to all projects.

After pushing new skills, pull them in with:

```text
/plugin marketplace update 4bs3nt-skills
```

## Local development

To have Claude Code read skills straight from a working copy (edits apply
without committing or pushing), register the local path instead:

```text
/plugin marketplace add /path/to/skills
```
