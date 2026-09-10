# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a starter template for "Claude Code Book" practice, intended as a Node.js/Playwright-based project. The repository is essentially a blank canvas — no application code or build tooling exists yet beyond the dev container setup.

## Dev Container

The project is configured for container-based development:

- Base image: `mcr.microsoft.com/devcontainers/base:bookworm` (Debian Bookworm)
- Pre-installed features: Node.js, GitHub CLI
- Post-create script installs Playwright Chromium dependencies:
  ```bash
  npx --yes playwright install-deps chromium
  ```

The workspace folder inside the container is `/workspaces/claude-code-book-template`.

## Current State

No `package.json`, build scripts, lint config, or test runner are set up yet. When adding these, Playwright (for Chromium browser automation) is the intended testing tool based on the devcontainer setup.
