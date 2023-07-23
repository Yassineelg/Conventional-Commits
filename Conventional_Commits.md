# Conventional Commits

## Introduction

Conventional Commits are a naming convention for commit messages used in version control systems like Git. This convention was created to standardize how commits are written, making communication among development team members more effective and simplifying the versioning automation process.

## Commit Structure

A Conventional Commit follows a specific structure, consisting of a header, an optional body, and an optional footer. Here's what the structure looks like:

```
<type>[optional(scope)]: <description>

[optional(body)]

[optional(footer)]
```

- **Type**: The commit type indicates the nature of the changes. Here are some commonly used types:
  - `feat`: Adding a new feature.
  - `fix`: Fixing a bug.
  - `docs`: Updating documentation.
  - `chore`: Maintenance tasks.
  - `test`: Adding or modifying tests.
  - `refactor`: Code restructuring without adding new features.
  - `config`: Adding or modifying configuration files.
  - `remove`: Removing code or files.
  - `perf`: Improving performance.

- **Scope (optional)**: The scope specifies the scope of the changes. It can be used to indicate the module, component, or functionality affected by the commit.

- **Description**: The description is a brief summary of the changes made by the commit. It should be concise and descriptive.

- **Body (optional)**: The commit body contains additional information about the changes made, providing more detailed context for the commit.

- **Footer (optional)**: The footer is used to reference issues, pull requests, or other metadata related to the commit.

## Example of a Conventional Commit

```
feat(authentication): add Google authentication
```

In this example:
- The commit type is `feat` for adding a new feature.
- The scope is `authentication`, indicating that the changes relate to authentication.
- The description is `add Google authentication`.

## Benefits of Conventional Commits

Conventional Commits offer several advantages:

1. **Clarity and Readability**: The standardized structure makes commit messages clear and easy to understand, even for team members unfamiliar with a specific project.

2. **Automation-Friendly**: With the predictable structure, automation tools can analyze commit messages to automatically generate release notes, changelogs, and other useful information.

3. **Enhanced Collaboration**: By using a common convention, developers can better understand the changes made by their colleagues, facilitating collaboration within the team.

## Example of Footer with References

```
fix(ui): fix alignment of toolbar buttons

Issue-Id: 123
Reviewed-by: John Doe
```

In this example, the footer uses custom metadata like "Issue-Id" to reference an internal project issue, and "Reviewed-by" to specify the name of the person who reviewed the code.

Remember, Conventional Commits can be adapted to the specific needs of your project, and it's essential to ensure that any convention you adopt is well-documented and understood by the development team.