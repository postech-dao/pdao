# PDAO Development Guide

## Commit Message Convention

```
<type>: do something
```

or

```
<type>: do something

It does something.
```

- Use imperative mood.
- Omit articles (`a/an` and `the`).
- Always put the proper `<type>`

### Types
From [angular project](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines)

1. build: Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)
1. ci: Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs)
1. docs: Documentation only changes
1. feat: A new feature
1. fix: A bug fix
1. perf: A code change that improves performance
1. refactor: A code change that neither fixes a bug nor adds a feature
1. style: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
1. test: Adding missing tests or correcting existing tests

## Pull Request Convention
- Use **rebase only** (No merge or squash).
- Push your works on your own forked repo, and make a **PR across forks**.
- Use the same title (head) and content (body) for a single-commit PR.
- When the PR resolves some issues, put `fixes #123` in the content of the PR, not in the commit messages.
- Conversation must be resolved by the commentor, not the PR author.
- Do not take the Github notifications as the communication channel; use Discord. 
