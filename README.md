# git-fiddle [![Build Status](https://travis-ci.com/felixSchl/git-fiddle.svg&branch=master)](https://travis-ci.com/felixSchl/git-fiddle)

`git-fiddle` is a wrapper around `git-rebase(1)` that allows editing of commit
information straight from the `git-rebase` editor, such as the author date,
author name and commit message. This makes it trivial to edit a whole range
of commits, shift them through time or alter ownership.

## Usage

Usage is almost identical to that of `git-rebase`.

```
$ git fiddle -h
git-fiddle

Edit commit meta information during an *interactive* rebase.

`git-fiddle(1)' is a lightweight wrapper around `git-rebase(1)' that
annotates each commit with it's *author* date, the author name, as well
as the commit message. Changes to any of these will then be applied
using a 'exec' script during the git-rebase sequence.

Usage:
  $SCRIPT [--[no-]messages] [args...]

Options:
  --no-messages Do not edit commit messages. Useful for quick edits to
                author or date.
  [args...]     These arguments are passed verbatim to git-rebase.
```

## License

<strong>git-fiddle</strong> is released under the **MIT LICENSE**.
See file `LICENSE` for a more detailed description of its terms.
