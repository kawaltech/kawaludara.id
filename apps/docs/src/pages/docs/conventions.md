---
title: Conventions
description: Commit message, GitHub issue, and pull request labels conventions.
---

Commit message, GitHub issue, and pull request label conventions. {% .lead %}

## Commit Messages

Understanding what's happening in a repository with many contributors like this and navigating between commits is essential.
Moreover, with various levels of contributors & their backgrounds, the commit messages can easily be confusing, and the structure may follow different approaches.

To overcome these issues, we adopt [Git commit conventions](https://www.conventionalcommits.org/en/) to allow contributors to add more semantic meaning to our Git history.
We use [commitlint](https://commitlint.js.org/) to lint the git commit messages.
To enforce it, we use a Git pre-commit hook to run the commitlint upon a Git commit command.
This configuration prevents committing the staged files if the commit message fails to comply with the conventions.

It's advisable to read the [commit conventions](https://www.conventionalcommits.org/en/v1.0.0) briefly to understand their other benefits further.
However, if you're having problems with it, you can use [this tool](https://commitlint.io/) to help.

Furthermore, please refer to the list of [commit types](#commit-types) and [scopes](#commit-scopes) we use to avoid adding a new scope with a similar meaning or synonym to the existing ones.

### Conventional Commits

The convention specification looks like this:

```txt
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

### Commit types

Here are what we use for the commit types:

- `build`
- `chore`
- `docs`
- `feat`
- `fix`
- `perf`
- `refactor`
- `style`
- `test`

### Commit scopes

Here are what we use for the scopes:

- `docs`
- `web`
- `ios`
- `android`
- `config`
  - `eslint`
  - `ts`
- `ui`
- `e2e`
- `security`
- `seo`

{% callout title="Note" %}
If there's a second level in a list, please use the lowest level only.
{% /callout %}

## Issue and Pull Request Labels

Issue labels are a tool to group issues into one or more categories. It helps us
track and manage issues and pull requests.

Please open an issue on
[`kawaltech/kawaludara.id`](https://github.com/kawaltech/kawaludara.id/issues)
if you have suggestions for new labels.

### Type of Issue and Issue State

| Label name                                                                                  | Description                                                                                                              |
| ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| [blocked](https://github.com/kawaltech/kawaludara.id/labels/blocked)                       | Issues blocked by something else.                                                                                        |
| [bug](https://github.com/kawaltech/kawaludara.id/labels/bug)                               | Confirmed bugs or reports that are very likely to be bugs.                                                               |
| [enhancement](https://github.com/kawaltech/kawaludara.id/labels/enhancement)               | New feature or request.                                                                                                  |
| [epic](https://github.com/kawaltech/kawaludara.id/labels/epic)                             | A master issue thread which contains other smaller issues.                                                               |
| [good first issue](https://github.com/kawaltech/kawaludara.id/labels/good%20first%20issue) | Less complex issues which would be good first issues to work on for users who want to contribute to Kelas Rumah Berbagi. |
| [help wanted](https://github.com/kawaltech/kawaludara.id/labels/help%20wanted)             | Issue that need extra attention.                                                                                         |
| [invalid](https://github.com/kawaltech/kawaludara.id/labels/invalid)                       | Issues which aren't valid (e.g. user errors).                                                                            |
| [question](https://github.com/kawaltech/kawaludara.id/labels/question)                     | More information needs to be collected about these problems or feature requests (e.g. steps to reproduce).               |
| [wontfix](https://github.com/kawaltech/kawaludara.id/labels/wontfix)                       | The Kelas Rumah Berbagi team will not fix these issues for now.                                                          |

### Topic Categories

| Label name                                                                        | Description                                   |
| --------------------------------------------------------------------------------- | --------------------------------------------- |
| [ci-cd](https://github.com/kawaltech/kawaludara.id/labels/ci-cd)                 | Continuous Integration & Continuous Delivery. |
| [design](https://github.com/kawaltech/kawaludara.id/labels/design)               | Issue related to design.                      |
| [documentation](https://github.com/kawaltech/kawaludara.id/labels/documentation) | Improvements or additions to documentation.   |
| [dx](https://github.com/kawaltech/kawaludara.id/labels/dx)                       | Developer Experience.                         |
| [ui](https://github.com/kawaltech/kawaludara.id/labels/ui)                       | User interface.                               |
| [ux](https://github.com/kawaltech/kawaludara.id/labels/ux)                       | User experience.                              |
| [seo](https://github.com/kawaltech/kawaludara.id/labels/seo)                     | Search engine optimization.                   |
| [scripting](https://github.com/kawaltech/kawaludara.id/labels/scripting)         | Issue related to the code.                    |
| [testing](https://github.com/kawaltech/kawaludara.id/labels/testing)             | Automated testing.                            |
