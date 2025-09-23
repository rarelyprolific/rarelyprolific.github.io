---
title: Git Commands
layout: post
---

- `git config --global fetch.prune true` - Automatically cleans up local references to branches which have been removed from the remote
repository when you **fetch** or **pull**. These are typically deleted in the remote when pull requests are completed.

- `git branch --merged main` - Shows all branches which have already been fully merged into **main**. This is useful for identifying branches
which are safe to delete in your local repository (i.e. completed pull requests).
