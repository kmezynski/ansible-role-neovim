# Contributing to Ansible Role: Neovim

Read our [Code of Conduct](./CODE_OF_CONDUCT.md) to keep our community
approachable and respectable.

In this guide, you will get an overview of the established standards in the
project and the contribution workflow, from opening an issue, creating a PR,
reviewing, and merging the PR.

## Getting started

For an overview of the project, read the [README](../README.md).
Keep in mind that this project adheres to the
[Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
specification, which has also been extended to define the naming pattern for
branch names, and a detailed explanation is presented in one of the following
subsections.

Here are some resources to help you get started with Ansible and open source
contributions:

- [Ansible Roles](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_reuse_roles.html)
- [Ansible Molecule](https://molecule.readthedocs.io/en/latest/getting-started/)
- [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
- [GitHub flow](https://docs.github.com/en/get-started/quickstart/github-flow)

### Issues

#### Create a new issue

If you spot a problem with the project, [search to see if an issue already exists](https://docs.github.com/en/github/searching-for-information-on-github/searching-on-github/searching-issues-and-pull-requests#search-by-the-title-body-or-comments).
If a related issue doesn't exist, you can open a new issue using a relevant
[issue form](https://github.com/kmezynski/ansible-role-neovim/issues/new/choose).

#### Solve an issue

Scan through our [existing issues](https://github.com/kmezynski/ansible-role-neovim/issues)
to find one that interests you. You can narrow down the search using `labels`
as filters. As a general rule, all issues are assigned to @kmezynski, but if
you find an issue to work on, you are welcome to open a PR with a fix.

### Make changes

1. Fork the repository.

- Using GitHub Desktop:

  - [Getting started with GitHub Desktop](https://docs.github.com/en/desktop/installing-and-configuring-github-desktop/getting-started-with-github-desktop)
    will guide you through setting up Desktop.
  - Once Desktop is set up, you can use it to
    [fork the repo](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/cloning-and-forking-repositories-from-github-desktop)!

- Using the command line:
  - [Fork the repo](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo#fork-an-example-repository)
    so that you can make your changes without affecting the original project
    until you're ready to merge them.

2. Install or update **Ansible** and **Molecule** to the newest version.

3. Create a new working branch and follow the recommended naming convention:
   `<type>/<subject>`. The `type` should follow the specification defined by
   **Conventional Commits**, while the `subject` should be a lowercase, imperative
   or keyword phrase that briefly describes the purpose of the branch.

### Commit your update

After making changes to the code, commit your changes once you are satisfied
with them. It's best to keep your commits small and focused on a particular
subject to make it easier for other to understand your changes. Additionally,
it's a good practise to perform a self-review to speed up the review process.
Make sure to follow the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
specification.

### Create a pull request

When you're finished with the changes, create a pull request (PR).

- Fill the template so that we can review your PR. This template helps
  reviewers understand your changes as well as the purpose of your pull request.
  Don't forget to link PR to issue if you are solving one.
- Enable the checkbox to allow maintainer edits so the branch can be updated
  for a merge. Once you submit your PR, a team member will review your proposal.
  We may ask questions or request additional information.
- We may ask for changes to be made before a PR can be merged, either using
  suggested changes or pull request comments. You can make any other changes in
  your fork, then commit them to your branch.
- As you update your PR and apply changes, mark each conversation as resolved.
  If you run into any merge issues, checkout this [git tutorial](https://github.com/skills/resolve-merge-conflicts)
  to help you resolve merge conflicts and other issues.

### Your PR is merged!

Congratulations! Thanks for contributing 🎉!
