# `gh weekly` GitHub CLI extension

[GitHub CLI](https://github.com/cli/cli) extension that generates a report in markdown listing the PRs you (or somebody else) worked on during the last week or so.

## Installation

```
gh extension install mgaitan/gh-weekly
```

Then run:

```
gh weekly
```

The full command line syntax is:

```
gh weekly [--author <author>] [--since <since>] [--org <org>]
```

By default the `--author` is `"@me"` (i.e you!), `--since` is `"7 days ago"` 
and `--org` is the owner of the repo you are currently running the command.

So, for example, what has our fellow pythonist [@pablogsal](https://github.com/pablogsal) 
been doing in the Python repos during the last 3 days?

```
$ gh weekly --author pablogsal --org python --since "3 days ago"
- [#105985](https://github.com/python/cpython/pull/105985) gh-98931: Add custom error messages to invalid import/from with multiple targets (MERGED)
- [#105962](https://github.com/python/cpython/pull/105962) gh-105960: Prevent stack overflows when using itertools.chain.from_iterable (CLOSED)
```
