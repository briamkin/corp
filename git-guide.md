# git guide

## git branches
We use the following conventions for branch names:
* feature/name-of-feature
* fix/name-of-fix
* refactor/name-of-refactor

## Commit messages
* Use the imperative sense – a good way to frame this tense is to finish the sentence "this commit will ...". For example:
  * Add MRR models
  * Fix typo in sessions model description
  * Update schema to v2 schema syntax
  * Upgrade project to dbt v0.13.0
* Commit early and commit often! As soon as a piece of your code works, commit it! This means that if, down the line, you introduce bad code, you can easily take your code back to the state it was in when it worked.
* Don't be afraid to squash commits on your local repository before (force) pushing them to your remote repository to tidy things up.

## Pull requests
A Pull Request (PR) should tackle a functional grouping of work. While it may be tempting to (for example) build MRR models _and_ add maintenance jobs in a single PR, they should be separate.
A good PR body explains the context of the changes to the code, as well as what the code does.
Useful things to include in a Pull Request are:
* Links to Trello cards
* Links to dbt docs that explain any new piece of functionality you have introduced
* A screenshot of the DAG for the new models you have built
If appropriate, you can use a PR Template to encourage others making PRs on the repo to do the same.

## Policy & procedure
* Reviewers should have 48 hours to complete a review, so plan ahead with the end of your sprint.
* If you have questions/problems, discuss them with your reviewer early. PRs are a good place to collaborate on code, so it is entirely appropriate to open a draft PR and use it as a tool to open up a discussion. If you're doing this, make sure you open your discussion early, rather than opening up discussion after you've done all the work.
