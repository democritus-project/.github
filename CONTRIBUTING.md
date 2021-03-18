# Contributing a PR 🏋️

Hello 👋 ! Thank you for your interest in contributing to this project; we couldn't do it without you, so thank you!

Here is a typical workflow for contributing... if you have *any* questions, please ask!

0. Decide what you want to work on (if you want to fix an issue, please comment on the issue asking us to assign it to you)
1. [Fork][fork] this repository
2. [Clone][clone] the forked repository locally
3. [Create a branch][branch]
    - We recommend starting your branch name with the issue number you are working on
    - We also recommend giving your branch a helpful name
    - A good branch name is `7-fix-lint-errors`; a bad one is `fix-stuff`
4. Make your code changes
    - This is the really fun part 😃
5. Write tests
    - Another fun part as you get to write some tests to show off your work 🚀
6. Push your changes to your fork
7. [Create a pull request][pr] from your fork to this repository
8. We'll review the updates you made and merge the PR!

# Local Development 🐳

This section describes how you can test, lint, and explore a project.

## Prerequisites

If you want to test, lint, or explore a project, make sure you have [docker][docker] and [docker-compose][docker-compose] installed (if you don't see: [installing docker][docker-install]).

Then you can use the **test**, **lint**, and **dev** docker compose services listed below!

## Test 🧪

To test this project, run the following command from the root directory of the project:

```shell
docker-compose run --rm test
```

Typically, this command will run [pytest][pytest-link] on the project's test suite. To view the details of what this command does, take a look at the `test` service in the project's `docker-compose.yml` file.

## Lint 🧹

To lint this project, run the following command from the root directory of the project:

```shell
docker-compose run --rm lint
```

Typically, this command will run a number of linters on the project's code with the goal of improving code quality and catching bugs before they are released (you can read more about the benefits of linting [here][linting-intro]). To view the details of what this command does, take a look at the `lint` service in the project's `docker-compose.yml` file.

## Explore 🔭

To explore a project, you can drop into a "dev" environment which is an [IPython][ipython] shell with the project and all its requirements loaded. To do this, run the following command from the root directory of the project:

```shell
docker-compose run --rm dev
```

To see what this command does, take a look at the `dev` service in the project's `docker-compose.yml` file.

# Questions? Please Ask!

If you have any follow-up questions, don't hesitate to ask! It takes practice to understand how to contribute to open-source software, so there is no shame in asking for help.

[fork]: https://docs.github.com/en/github/getting-started-with-github/fork-a-repo
[clone]: https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository
[branch]: https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging
[pr]: https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request-from-a-fork
[pytest-link]: https://docs.pytest.org/en/stable/
[docker-compose]: https://docs.docker.com/compose/
[docker-install]: https://docs.docker.com/get-docker/
[docker]: https://www.docker.com/get-started
[linting-intro]: https://dbader.org/blog/python-code-linting
[ipython]: https://ipython.org/
