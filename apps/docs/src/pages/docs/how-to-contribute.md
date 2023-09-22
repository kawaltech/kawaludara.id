---
title: How to contribute
description: Contributing to Kawal Udara Monorepo.
---

Contributing to Kawal Udara Monorepo. {% .lead %}

In this project, we heavily utilise GitHub features to document and signal any progress in the development process.

## Understanding GitHub Projects

In 2021, GitHub launched a new [Project planning feature](https://github.com/features/issues) in beta. You can read [GitHub's official document](https://docs.github.com/en/issues/trying-out-the-new-projects-experience/about-projects) about this new feature.

We are trying to utilise this new feature to manage our issues better. Here is the way we are using it in this project.

### Backlog

To find the state of all issues, please visit the [Kawal Udara Monorepo board](https://github.com/orgs/kawaltech/projects/1/views/1). These are what each column on the board means:

| Status        | Description                                                                                                                |
| ------------- | -------------------------------------------------------------------------------------------------------------------------- |
| 🆕 New        | It is newly created, usually has incomplete descriptions                                                                   |
| 📋 Backlog    | The description is complete, but not all the prerequisites are fulfilled.                                                  |
| 🔖 Ready      | It is ready for development                                                                                                |
| 🏗 In Progress | Somebody has started working on it, indicated by a [draft PR](#creating-a-draft-pull-request) linked                       |
| 👀 In Review  | The maintainer is reviewing the PR, indicated by a [PR ready for review](#marking-pull-request-as-ready-for-review) linked |
| ✅ Done       | The PR has been merged to the `main` branch and deployed                                                                   |

### Epics list

To visualise the list of epics covering all issues in this project and understand the overall state of this project, please visit the [Epics list](https://github.com/orgs/kawaltech/projects/1/views/4) tab.

## Finding or creating issues

Most contributions start from defining issues. Anyone can open an issue for discussion. You can head to [this link](https://guides.github.com/features/issues/) for a deep understanding of the Issues. Specifically, you can start finding several Issues in [our Issues tab](https://github.com/kawaltech/kawaludara.id/issues). There are only two categories in the Issues section, Open and Closed.

### Open Issues

Open Issues are issues that need more attention, and we need to work on them. Contributors should pick any of the Open Issues and start working on them.

### Closed Issues

Closed Issues are issues that have been completed or don't need further action. We can reopen Closed issues if contributors find any issues related to them sometime in the future.

Please pay attention to every issue attribute. Other contributors might reference every issue through [Linked Pull Requests](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue).
If an issue has a linked pull request, someone is currently handling it.
We encourage contributors to submit a [draft pull request](https://github.blog/2019-02-14-introducing-draft-pull-requests/) to avoid redundant work when working on an issue.

### For beginners: `good first issue` label

As mentioned [here](https://github.blog/2020-01-22-browse-good-first-issues-to-start-contributing-to-open-source/), GitHub treats the `good first issue` label in a particular way to help beginners contribute to an open-source project.
The `good first issue` label informed us about the difficulty level of an issue. It means that an issue with a `good first issue` label suits perfectly for contributors who would like to contribute to an open-source project.

How to find issues with `good first issue` label:

1. The easiest way is to go into the `github.com/<owner>/<repository>/contribute` link. In this case, you can go to [this link](https://github.com/kawaltech/kawaludara.id/contribute).
   That link will list all the issues with the `good first issue` label.
2. Another way is to head to the [Issues](https://github.com/kawaltech/kawaludara.id/issues) repository section and click the Labels section beside Milestones.
   There you can see a lot of labels for the issues in the repository. Then find and click the `good first issue` label.

## Working on issues

### Getting ready

Before working on an issue, please make sure to:

1. Fork the repo properly. Even if you have done it before, we still advise you to read/skim
   [the official guide](https://docs.github.com/en/get-started/quickstart/fork-a-repo#forking-a-repository).
2. Clone **your forked repository** and set it up by following the
   [Getting Started guide](https://github.com/kawaltech/kawaludara.id#getting-started).
3. Check any open [pull requests](https://github.com/kawaltech/kawaludara.id/pulls) so that no one is working on the issue.
4. Create a new branch from the `main` branch. It is essential [to allow the maintainers to update the code changes directly](https://twitter.com/kentcdodds/status/1683681287918465025) when they have suggestions.

### Issue assignment & communication

Once you're ready with your branch and have something to contribute, you'll want to let everyone know you are working on the issue. To communicate this, we are using GitHub's Draft Pull Requests.

Draft Pull Request is like a regular Pull Request, but we can't merge it until
we mark it as "ready for review". It signals other contributors that
[it's a work in progress](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/changing-the-stage-of-a-pull-request).
It is necessary to signal other contributors that the work for the particular
issue has started and is still in progress. Also, it is a better approach to
use as a communication tool between contributors because we can provide
additional information other than viewing the changed files.

{% callout type="warning" title="Attention" %}
When you have at least one commit, _creating a Draft Pull Request is crucial_ to let everyone know that we have assigned the issue to you.
{% /callout %}

### Creating a Draft Pull Request

Steps to creating a Draft Pull Request:

1. Commit and push your new changes into the remote repository. Please refer to
   [@commitlint/config-conventional](https://github.com/conventional-changelog/commitlint/tree/master/@commitlint/config-conventional)
   for your commit message, or you can use [commitlint.io](https://commitlint.io/) to assist you in composing the commit message.
2. Head to the Pull requests section on your forked repository, and hit New pull request.
   {% figure src="https://user-images.githubusercontent.com/46013258/126284390-c2bd1aa6-fdc2-4aa6-a945-031f02db038e.png" alt="Pull requests tab" caption="Pull requests tab" /%}
3. Select your forked repository for the head repository, and compare with the branch in which you are changing.
   {% figure src="https://user-images.githubusercontent.com/46013258/126285036-27b49325-62a2-4a6c-b216-5bae261788da.png" alt="Create pull request button" caption="Create pull request button" /%}
4. Put a clear title and description in your pull request. Make sure the
   description follows [our guide below](#formatting-pull-request-description).
   {% figure src="https://user-images.githubusercontent.com/46013258/126286179-04341e30-1224-49cb-9b9a-3c3aee99c308.png" alt="Create draft pull request" caption="Create draft pull request" /%}
5. Choose `Create draft pull request`` (like in the image above) and hit the green button.
6. Don't forget to mark your Draft Pull Request as Ready for review after you commit all the changes.

### Formatting Pull Request description

To properly
[link a pull request to an issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue),
there is one tiny requirement text to put in a Pull Request description. Please
make sure to mention the issue that you're working on correctly. Replace this
text `<!-- mention the issue that you're trying to close with this PR -->` from
the template with the issue number. Example:

```markdown
Closes #318

## Description

Update **`Start working on Issues`** section with clearer instructions on
getting ready to work on an issue.
```

### Marking Pull Request as Ready for Review

When you have finished working on the issue, you can mark your Draft Pull Request as Ready for review. This action will notify other contributors that the issue is ready for review. Please follow [these steps](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/changing-the-stage-of-a-pull-request#marking-a-pull-request-as-ready-for-review) to do so.

### Disabling GitHub Actions

We recommend contributors turn off GitHub action on your forked repository.

1. Go to Setting on your forked repository
2. Choose Action on the sidebar
3. Disable Actions
   {% figure src="https://user-images.githubusercontent.com/35433920/129485485-ca7d1202-5dbc-46f7-b823-978d3f4ed600.png" alt="Disable GitHub Actions" caption="Disable GitHub Actions" /%}
