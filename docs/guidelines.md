# Project Guidelines

## Code Reviews
All code has been reviewed by someone other than the author.
This can be part of the development process where pair programming is
practiced.  For pull requests into the master branch there are processes in
place to enforce code reviews and merge approvals.  Only reviewed code,
unchanged from what has been approved, is merged.

## Testing
Developers can build code locally.  Developers can run tests (unit test and
functional test) locally.  Tests are repeatable and automated.  Under Test
Driven Development tests are developed before the code.  No code is to be
delivered without having tests that validate the code.

## Documentation

Code has user-facing documentation on how to build, install and use.
Documentation is delivered with code in markdown format.  The markdown content
is used by both GitHub and ReadTheDocs, and must generate correctly under both.

## Pull Requests

Changes to the GitHub repository contents will follow the checklists outlined
[here](maintainers_corner.md#github).  Maintainers ensure that the PRs satisfy
those requirements before an approval.

Developers will follow the [GitHub
Flow](https://guides.github.com/introduction/flow/) model for PR submissions.
Howeber, Ocopea branching is not allowed.  GitHub supports cloning a repository
where changes can be made.  PRs are submitted from a cloned or forked
repository, not a branch of the project.  

Before submitting a PR, developers should ensure that the submission has been:

* rebased relative the the current master
* reduced to a single commit

