# Contributing

I value contributions to my projects that can be provided: bug reports, feature
requests, pull requests and discussions. All participation in these projects is
subject to the Code of Conduct in the repository or described in
<https://github.com/halosttue/.github>.

I may not receive a notification of new or updated issues or pull requests or
unless I am tagged (`@halostatue`); this should be used sparingly or if at least
five days have passed.

Code contributions are always encouraged, but I have a few recommendations:

- Code changes **must** have tests if there is a test suite.

- Code changes **should** match my coding style. In many projects, this is
  assisted with a common formatter / style checker. If there is not a code
  formatter, use your best judgement.

  - Elixir projects use `mix format` and [credo][credo].
  - Rust projects use `rustfmt`.
  - Go projects use `go fmt`.
  - Ruby projects use [standard][standardrb].
  - Python projects use [ruff][ruff].
  - Typescript projects use [biome][biome].

- Pull requests should be on a thoughtfully-named topic branch with separate
  commits representing logical chunks. Most of my projects are using rebase or
  fast-forward-only merges moving forward.

- Commit messages should be [carefully considered][qcm]. I will accept variants
  of [conventional commits][cc]. Unless otherwise noted in the project
  documentation, my conventions are:

  - commit types: `fix`, `feat`, `chore`, `ci`, `docs`, `deps`, `test`
  - commit scopes: do not use
  - breaking changes: **must** be specified as a git trailer; do not use the
    trailing `!`
  - when using conventional commit types, the commit subject line **may** exceed
    50 characters, but **should not** exceed the 52 characters plus length of
    the commit type.

- Changes **should** include updated documentation, if appropriate.

- Contributors **should** update the changelog file (usually named
  `Changelog.md` or `History.md`). If there is no section at the top of the file
  for unreleased changes, one should be added.

- Version numbers **should not** be updated by non-maintainers.

- Submit a GitHub pull request with your changes. There will likely be status
  checks that must pass before your pull request can be merged.

[biome]: https://biomejs.dev
[cc]: https://www.conventionalcommits.org/en/v1.0.0
[credo]: https://github.com/rrrene/credo
[qcm]: http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html
[ruff]: https://github.com/astral-sh/ruff
[standardrb]: https://github.com/standardrb/standard
