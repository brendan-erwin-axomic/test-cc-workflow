# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Tooling

This project uses [Devbox](https://www.jetify.com/devbox) for tooling and scripts. Use `devbox run` to install tools and run project scripts. When you need a CLI tool, add it via devbox rather than installing globally.

Use `devbox run` to install any tooling you need whenever you need it — it's there so you can work quickly.

## Workflow (cc-workflow)

The cc-workflow plugin is enabled. Available devbox scripts:

- **Work items**: `devbox run work:items`, `devbox run work:item <id>`, `devbox run work:item:create`, `devbox run work:item:close`
- **Work containers** (epics/groups): `devbox run work:containers`, `devbox run work:container <id>`, `devbox run work:container:create`, `devbox run work:container:close`
- **Labels**: `devbox run work:label:create`
- **PRs**: `devbox run pr:create`, `devbox run pr:list`, `devbox run pr:check`, `devbox run pr:ready`, `devbox run pr:merge`
- **Utilities**: `devbox run text:slugify`, `devbox run ccw-refresh-config`

## Permissions

- `devbox run *` commands are pre-approved
- `devbox run -- *` commands are denied (use the script names directly)
