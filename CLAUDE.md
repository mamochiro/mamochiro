# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a **GitHub profile README repository** (`mamochiro/mamochiro`). It contains a personal profile page displayed on the GitHub user profile at github.com/mamochiro. There is no application code, build system, or test suite.

## Structure

- `README.md` — The profile page content (HTML + Markdown), featuring bio, tech stack badges, GitHub stats widgets, and a contribution snake animation.
- `.github/workflows/snake.yml` — GitHub Actions workflow that runs daily (via `Platane/snk@v3`) to generate contribution grid snake SVGs, pushed to the `output` branch.

## Key Details

- Images use external badge/icon services (`shields.io`, `devicons`, `readme-typing-svg.demolab.com`, `github-readme-stats.vercel.app`). Do not host these locally.
- The snake animation SVGs are generated on the `output` branch and referenced via `raw.githubusercontent.com` URLs. Do not commit SVGs to `main`.
- The README uses `<picture>` + `<source>` elements for dark/light mode support.
