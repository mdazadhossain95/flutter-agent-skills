# Contributing to Flutter Skills

We'd love to accept your patches and contributions to this project.

## Before you begin

### Sign our Contributor License Agreement

Contributions to this project must be accompanied by a
[Contributor License Agreement](https://cla.developers.google.com/about) (CLA).

You (or your employer) retain the copyright to your contribution; this simply gives us permission to use and redistribute your contributions as part of the project.

If you or your current employer have already signed the Google CLA (even if it was for a different project), you probably don't need to do it again.

Visit <https://cla.developers.google.com/> to see your current agreements or to sign a new one.

### Review our community guidelines

Please follow
[Flutter contributor guidelines](https://github.com/flutter/flutter/blob/master/CONTRIBUTING.md).

## Contribution process

### Code reviews

All submissions, including submissions by project members, require review. We
use GitHub pull requests for this purpose. Consult
[GitHub Help](https://help.github.com/articles/about-pull-requests/) for more
information on using pull requests.

## Adding a New Skill

To add a new skill to the repository, follow these steps. Note that both generation and validation require the `GEMINI_API_KEY` environment variable to be set.

1. **Define the Skill**: Add a new entry to the `resources/flutter_skills.yaml` file. Follow the style of existing entries (use short descriptions and summarized instructions).
2. **Generate the Skill**: Run the generation tool from the repository root:
   ```bash
   dart run tool/generator/bin/skills.dart generate-skill --skill <skill-name> -d tool/dart_skills_lint/skills resources/flutter_skills.yaml
   ```
3. **Validate the Skill**: Run the validation tool to ensure it meets the standards:
   ```bash
   dart run tool/generator/bin/skills.dart validate-skill --skill <skill-name> -d tool/dart_skills_lint/skills resources/flutter_skills.yaml
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