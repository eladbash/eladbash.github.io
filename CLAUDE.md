# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Personal portfolio website for eladbash.com. Pure static HTML/CSS site (no build system, no JavaScript framework, no package manager).

## Architecture

Single-page static site:
- `index.html` — entire site content (Bootstrap 4, Google Fonts/Roboto)
- `styles.css` — custom styles on top of Bootstrap
- `images/` — static assets

No build step, no transpilation, no dependencies to install.

## Deployment

- **Hosting:** AWS S3 bucket serving eladbash.com behind CloudFront CDN
- **CI/CD:** AWS CodePipeline auto-deploys on push to `master` branch (GitHub integration)
- **Cache:** If changes don't appear after push, invalidate the CloudFront cache
