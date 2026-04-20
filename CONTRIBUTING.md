# Contributing to Flutter Agent Skills

We'd love to accept your patches and contributions to this project. This repository extends the official [Flutter Skills](https://github.com/flutter/skills) with custom, MIT-licensed skills designed for AI agent workflows.

## Before you begin

### Code of Conduct

Please follow our [Code of Conduct](CODE_OF_CONDUCT.md) in all interactions.

### Community guidelines

This project values inclusivity, professionalism, and constructive collaboration. All contributors should:
- Be respectful and considerate in discussions
- Provide clear, actionable feedback
- Test changes before submission
- Document your work

## Contribution process

### Code reviews

All submissions, including submissions by project members, require review. We use GitHub pull requests for this purpose. Consult [GitHub Help](https://help.github.com/articles/about-pull-requests/) for more information on using pull requests.

## Adding a New Skill

To add a new custom skill to this repository, follow these steps:

### 1. Create the skill folder and file

```bash
mkdir -p skills/flutter-your-skill-name
touch skills/flutter-your-skill-name/SKILL.md
```

### 2. Write the SKILL.md file

Follow the skill specification with YAML frontmatter:

```yaml
---
name: flutter-your-skill-name
description: Brief description of what this skill does. Use when... (50-100 words)
instructions: |
  Detailed step-by-step instructions for how to use this skill.
  Can span multiple paragraphs.
resources:
  - https://docs.flutter.dev/app-architecture
  - https://docs.flutter.dev/cookbook
---

# Optional markdown body content (if instructions need structure)
Additional guidance, examples, or use cases.
```

**Requirements:**
- Skill name must start with `flutter-` and use kebab-case (lowercase, hyphens)
- Description required (brief, action-oriented)
- Instructions required (clear, actionable)
- Resources required (at least one reference link)

### 3. Register the skill in config

Add an entry to `resources/flutter_agent_skills.yaml`:

```yaml
- name: flutter-your-skill-name
  description: Your skill description
  instructions: |
    Your instructions from SKILL.md
  resources:
    - https://docs.flutter.dev/app-architecture
```

### 4. Validate the skill

Run the linter to ensure your skill meets standards:

```bash
cd tool/dart_skills_lint
dart run bin/cli.dart --skills-directory ../../skills
cd ../..
```

The skill must pass all checks:
- Naming convention (flutter-* kebab-case)
- Metadata validation (name, description, instructions, resources present)
- File structure (SKILL.md exists)

### 5. Update README.md

Add your skill to the appropriate table in [README.md](README.md):

- **Official Skills**: 22 official Flutter skills (BSD-3-Clause licensed) - do not add here
- **Extended Skills**: Custom skills (MIT-licensed) - add your new skill here

### 6. Test and submit

```bash
# Create a feature branch
git checkout -b feature/add-flutter-your-skill-name

# Commit your changes
git add -A
git commit -m "feat: add flutter-your-skill-name skill"

# Push and create a PR
git push -u origin feature/add-flutter-your-skill-name
```

## Issue triage

We regularly triage issues by looking at newly filed issues and determining what we should do about each of them. Triage issues as follows:

- Open the [list of untriaged issues][untriaged_list].
- For each issue in the list, do one of:
  - If we don't plan to fix the issue, close it with an explanation.
  - If we plan to fix the issue, add the `triaged` label and assign a priority: [P0][P0], [P1][P1], [P2][P2], or [P3][P3]. If you don't know which priority to assign, apply `P2`. If an issue is `P0` or `P1`, add it to a milestone.

At the end of a triage session, the untriaged issue list should be as close to empty as possible.

[untriaged_list]: https://github.com/flutter/skills/issues?q=is%3Aissue+state%3Aopen+-label%3Atriaged
[P0]: https://github.com/flutter/skills/labels?q=P0
[P1]: https://github.com/flutter/skills/labels?q=P1
[P2]: https://github.com/flutter/skills/labels?q=P2
[P3]: https://github.com/flutter/skills/labels?q=P3