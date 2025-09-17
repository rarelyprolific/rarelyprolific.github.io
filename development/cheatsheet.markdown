---
title: Cheatsheet
layout: post
---

Modern software development has a bewildering level of choice. Sometimes an opinionated, pre-configured tool can get you coding the stuff
you really want to be working on faster.

This is currently what works for me:

## Development Tools

- **Visual Studio** for C# development.
- **VS Code** (with plugins) for everything else.
- **Docker Desktop** (or another container tool).
- **k9s** for interacting with Kubernetes using a lightning fast terminal based UI.

## VS Code Plugins

- **markdownlint** to make formatting markdown easy.

## Other

- **Obsidian** for making notes and capturing ideas.

## Git Commands

- `git config --global fetch.prune true` - Automatically cleans up local references to branches which have been removed from the remote
repository when you **fetch** or **pull**. These are typically deleted in the remote when pull requests are completed.

- `git branch --merged main` - Shows all branches which have already been fully merged into **main**. This is useful for identifying branches
which are safe to delete in your local repository (i.e. completed pull requests).

## k9s Commands

- `:ctx` - Select Kubernetes context.
- `:ns` - Select Kubernetes namespace.
