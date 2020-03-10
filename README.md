# Gitbook Publish Action

![Build Status](https://github.com/dzoladz/gitbook-publisher/workflows/build/badge.svg)

This action publishes a GitBook to GitHub pages.

The source branch is `master`, and the target branch is `gh-pages`. If `gh-pages` does not exist, it will be created automatically.

## How to Use
- Copy this project to a new repo.
- Change `README.md` to the first page for the book.
- Change `SUMMARY.md` to the table of contents for the book.
- Update project url in [`book.json`].
- Render GitBook and publish to branch `gh-pages` by running [`bin/publish.sh`].
- After running `publish.sh` the first time, pushing changed to `master` will trigger a new build of the GitBook

### Creating access token
- This action requires a [personal access token (PAT)](https://help.github.com/en/github/authenticating-to-github/creating-a-personal-access-token-for-the-command-line#creating-a-token). The value of the PAT must be used to create a [GitHub secret](https://help.github.com/en/actions/configuring-and-managing-workflows/creating-and-storing-encrypted-secrets#creating-encrypted-secrets) with the key name of `PERSONAL_TOKEN`.

### Caveat
Repo must be public to generate the GitBook
