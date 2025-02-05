## Unconventional Commits

Commit messages for humans.

This is a Github Action that fails the build if the commits are written using [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/#specification).

## Usage

```yml
name: My workflow

on: [push]

jobs:
  my-job:
    runs-on: ubuntu-latest
    steps:
    - uses: adamu/unconventional_commits@v1
```

## Example failure

```
Run adamu/unconventional_commits@v1
...
Found conventional commit:
chore: rewrite the core logic and add some bugs
Error: Process completed with exit code 1.
```

## Why

Conventional commits are busywork, obfuscate the commit log, and suck the joy out of the creative process.

Use this action to catch any conventional commits that may sneak into your project and
defend your humanity.

## TODO

Option to automatically rewrite commits messages without the conventional part.
