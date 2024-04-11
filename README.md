# Android-Code-Exercise

## Project to develop:

- [Articles App](https://docs.google.com/document/d/1VX3cyOEqJ4hiRP2kogLYvMeRcppggpTNWCcVnQSzGMM)

## Related technologies:

- MVVM
  * Concept: [https://developer.android.com/topic/libraries/architecture/viewmodel](https://developer.android.com/topic/libraries/architecture/viewmodel)
  * Usage: [https://www.geeksforgeeks.org/mvvm-model-view-viewmodel-architecture-pattern-in-android/](https://www.geeksforgeeks.org/mvvm-model-view-viewmodel-architecture-pattern-in-android/)
- Lifecycles
  * Concept: [https://developer.android.com/topic/libraries/architecture/lifecycle](https://developer.android.com/topic/libraries/architecture/lifecycle)
- Coroutines:
  * Concept: [https://developer.android.com/kotlin/coroutines](https://developer.android.com/kotlin/coroutines)
  * Exercise: [https://developer.android.com/codelabs/kotlin-coroutines](https://developer.android.com/codelabs/kotlin-coroutines)
- ViewBinding
  * Concept: [https://developer.android.com/topic/libraries/view-binding](https://developer.android.com/topic/libraries/view-binding)

## Development preparation

To help with scoping the project, the development can be split into smaller "tickets". These tickets can be created here on [GitHub as Issues](https://github.com/FutureWorkshops/Android-Code-Exercise/issues).

## Development Flow

1. Choose a ticket to start tackling
2. Develop the feature using a Feature Branch starting from the main
3. When the feature is done, create a Pull Request to integrate the change into the main branch

## Branching

Using Git branches allows the features to be isolated during development, and allows the PR moment for a CI/CD to validate changes before reaching the main code.
A good pattern for the branch is to use `feature`, `chore` or `bug` to indicate the motivation for the change, followed by a more descriptive task. For example:

```sh
git checkout -b feature/login_page
git checkout -b chore/update_strings
git checkout -b bug/crash_when_refreshing_list
```

## Pull Request

The Pull Request is an opportunity to have the code pair-reviewed before merging. The goal of pair review is to minimise legacy code, improve security and catch small errors or improvements.
During the Pull Request review, the reviewer may add "non-blocker" comments with questions or improvements to be tackled at a later stage. Or, if any more serious issue is seen, a "blocker" comment.

The Pull Request comment area is a change for the author of the PR to give more context to the reviewer of the code, to ensure that the reader can better understand the motivation and choices made.

```markdown
# Task

[Login Page](https://github.com/FutureWorkshops/Android-Code-Exercise/issues/1)

# Notes

- The login view was created following the UX/UI designed in [Figma](https://figma.com/....)
- The tokens are being stored on SecuredSharePreferences
...

# Demonstration

![login_view](https://github.com/....)
```
