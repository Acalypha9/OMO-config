# OMO Config

This repository contains a publishable snapshot of my OpenCode configuration.

## Included files

- `opencode.json` - main OpenCode config, including providers, MCP setup, and model definitions
- `oh-my-opencode.json` - plugin-specific settings for browser automation, LSP, agents, and background task behavior
- `antigravity.json` - safe Antigravity auth behavior settings without account credentials
- `package.json` - plugin dependency manifest
- `bun.lock` - lockfile for the published dependency version
- `.gitignore` - excludes secrets, local caches, backups, and installed dependencies

## Excluded files

This repo intentionally does not publish local-only or sensitive data, including:

- `antigravity-accounts.json`
- `backup/`
- `node_modules/`
- temporary auth/cache files covered by `.gitignore`

## Notes

- The config enables the `oh-my-opencode` and `opencode-antigravity-auth` plugins.
- The published settings include a local `dart mcp-server` entry in `opencode.json`.
- You may need to adjust local paths, credentials, or installed tools before reusing this setup on another machine.
