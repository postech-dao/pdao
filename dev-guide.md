# PDAO Development Guide

## Commit Message Convention

```
<type>: <subject>
```

or

```
<type>: <subject>

<description>
```

- Always put the proper `<type>`
- `<subject>`
  - summarize your change
  - use imperative mood.
  - Omit articles (`a/an` and `the`).
  - should not exceed 75 characters
  - must start with lowercase
- `<description>` 
  - detailed explantion of your change

### Types
From [angular project](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines)

1. build: Changes that affect the build system or external dependencies 
2. ci: Changes to our CI configuration files and scripts 
3. docs: Documentation only changes
4. feat: A new feature
5. fix: A bug fix
6. perf: A code change that improves performance
7. refactor: A code change that neither fixes a bug nor adds a feature
8. style: Changes that do not affect the meaning of the code 
9. test: Adding missing tests or correcting existing tests
10. revert: Revert commit it should begin with `revert: `, followed by the header of the reverted commit. 
`<description>` must contain `This reverts commit <hash>.`

### Examples
```
feat: add account check logic

We have to verify 3 things here:
1. blah
2. blah
3. blah
```

## Pull Request Convention
- For the title, use imperative mood.
- Use **rebase only** (No merge or squash).
- Push your works on your own forked repo, and make a **PR across forks**.
- Use the same title (head) and content (body) for a single-commit PR.
- When the PR resolves some issues, put `fixes #123` in the content of the PR, not in the commit messages.
- Conversation must be resolved by the commentor, not the PR author.
- Do not take the Github notifications as the communication channel; use Discord. 


## Rust
### Use
Use a single chunk of `use`.

```rust
use a;
use b;
use c;
```
not
```rust
use a;
use b;

use c;
```

### `Rc` & `Arc`
Use `Rc::clone(&object)`:
```rust
let object = std::sync::Rc::new(inner_object);
// Explicit cloning of `Rc`.
let another_object = std::sync::Rc::clone(&object);
```
Do not use confusing `object.clone()`:
```rust
let object = std::sync::Rc::new(inner_object);
// This can be seen as cloning the inner object, not cloning the `Rc`, to other reviewers.
let another_object = object.clone();
```

## Naming & Versioning
A crate name must start with `pdao-`, except those crates in the `simperby` project (they're for general purpose).
