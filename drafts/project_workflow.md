# Project Workflow

This (draft) document includes some guidelines to set up and follow for
PracticeCraft projects.

## Project Management

- I suggest a very simple form of Kanban board with 3 lists:
    + To-Do
    + In Progress
    + Done
- Each card on the list should have a tag that marks it as a feature, a fix, or
a chore.
- This can be done using GitHub Projects, which has the advantage of converting
these cards to issues directly.

## Commit Message Style

- One of two choices to consider. I suggest choosing one and sticking to it for
all projects.
    1. [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
    2. A set of guidelines similar to the ones
       [here](https://initialcommit.com/blog/git-commit-messages-best-practices)
   
## CI

- All projects should have CI to enforce formatting, test passing, etc.
- We could set up a GitHub Action for each language to be used as a template.
- We could add optional setup for pre-commit hooks. Since hooks are specific to
local repos and not the GitHub one, we would only write a script and recommend
using it.

## Branches & PRs

- We could suggest a naming convention for branches.
- PRs must pass a code review (I think there is a way to enforce this on
GitHub).
- We could set up a Contribution Guide template that shows when opening the
Issues and PRs pages. It should point to the [PR
guide](https://wipdev.netlify.app/posts/collaboration-on-github/) among other
guidelines if any (e.g., we could suggest rebasing and squashing a branch
before sending the PR).

## Documentation & Testing

- The project README should follow the
[template](https://github.com/PracticeCraft/project-readme-template) we have.
- We need to ensure somehow that docs and testing are part of the code review.
