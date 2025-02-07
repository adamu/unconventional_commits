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

<img width="429" alt="image" src="https://github.com/user-attachments/assets/39d51c05-325b-4554-b035-92743365b14c" />

## Why

Conventional commits are busywork, obfuscate the commit log, and suck the joy out of the creative process.

Use this action to catch any conventional commits that may sneak into your project and
defend your humanity.

## TODO

Option to automatically rewrite commits messages without the conventional part.
