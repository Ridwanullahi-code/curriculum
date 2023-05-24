# Linters

## Learning objectives
- Understand the importance of code standards and linters.

### Estimated time: 0.5h

## Description

A linter is a tool that analyzes your *source code* to flag programming errors, bugs, stylistic errors, and suspicious constructs (source: [Wikipedia](https://en.wikipedia.org/wiki/Lint_(software))).

You can find linters for most programming languages, such as [Rubocop](https://www.rubocop.org/) for Ruby or [ESLint](https://eslint.org/) for JavaScript.

## Why are linters important?

There are a few reasons for using linters:

1. Catching syntax errors is more efficient. There is no need to debug simple mistakes like typos - the linter does it for you.
2. The entire codebase looks like it was written by one person.
3. Programmers can focus on solving problems instead of cleaning up the code.

As programmers, you will be part of a team. Agreeing on a set of [coding standards](https://en.wikipedia.org/wiki/Extreme_programming_practices#Coding_standard) is key to create quality code as a team, and linters will facilitate this task.


## How can I use linters in my code base?

There are many ways you can integrate a linter in your programming workflow:

- text editor plugins
- GitHub Actions
- GitHub apps


At Microverse, you are going to use linters in every single project that you develop. Please learn more about linters and how to include them on your repository [in our linters documentation](https://github.com/microverseinc/linters-config).

## Guidelines for using linters at Microverse

- You **should not change the `config` files** copied from the `linters-config` repo. They represent configuration shared between all students at Microverse.
- **Do not overuse linter disable comments**, i.e. `eslint-ignore <rule-to-be-ignored>` or `# rubocop:disable <rule-to-be-disabled>`. Disabling rules multiple times in the same file, or disabling easy to fix rules such as `no-console`, `no-alert`, `Layout/LineLength`, `Style/GuardClause`, etc, should be avoided. Linter rules are meant to catch bad code and enforce best practices.
- If you request a review for a project with linter errors, **your request will be invalidated.**

In each Microverse project you have a reminder about linters and a link to the correct config files.

## Additional Materials
- Here is an optional guide [explaining linters in greater detail](https://www.testim.io/blog/what-is-a-linter-heres-a-definition-and-quick-start-guide/) by Testim if you would like to learn more about linters.

------

_If you spot any bugs or issues in this activity, you can [open an issue with your proposed change](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/git-github/articles/open_issue.md)._
