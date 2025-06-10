# minimal-reproduction-template

First, read the [Renovate minimal reproduction instructions](https://github.com/renovatebot/renovate/blob/main/docs/development/minimal-reproductions.md).

Then replace the current `h1` with the Renovate Issue/Discussion number.

## Current behavior

The contents of `uv.lock` are erased when incrementing the package's `requires-python` then running `uv lock --upgrade-package python` (which is the command that `renovate` runs to update the lockfile)

[Example renovate PR](https://github.com/nrlulz/renovate-bug-repro/pull/1/files)

[Renovate log](./log.json)

## Expected behavior

`uv.lock` is updated with the new requires-python constraint and no other changes.

## Link to the Renovate issue or Discussion

Put your link to the Renovate issue or Discussion here.
