# Gitbook Publish Action

![Build Status](https://github.com/dzoladz/gitbook-publisher/workflows/build/badge.svg)

This action publishes a gitbook to github pages.

The source branch is `master`, and the target branch is `gh-pages`. If `gh-pages` does not exist, it will be created automatically.

## How to Use
- Copy this project to a new repo.
- Change `README.md` to the first page for the book.
- Change `SUMMARY.md` to the table of contents for the book.
- Update project url in [`book.json`](book.json).
- Render gitbook and publish to branch `gh-pages` by running [`bin/publish-gh-pages.sh`](bin/publish-gh-pages.sh).
- Happy writing.
