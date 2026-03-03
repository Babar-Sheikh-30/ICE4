# GitHub Actions Lab

## Overview
This repository demonstrates two GitHub Actions workflows:

- **Dependent Jobs Workflow**: Shows job dependencies and ordered execution using `needs`.
- **Multi-Platform Workflow**: Runs independent jobs in parallel across Linux, Windows, and macOS.

## Workflow 1: Dependent Jobs (`dependent-jobs.yml`)
**Purpose:** Enforces a strict job order: build → test → deploy.

**Key concepts demonstrated:**
- `needs` to define job dependencies
- `runs-on` to select the GitHub-hosted runner OS
- Meaningful step names and simulated work

## Workflow 2: Multi-Platform (`multi-platform.yml`)
**Purpose:** Runs three independent jobs simultaneously on different operating systems.

**Key concepts demonstrated:**
- Parallel jobs by omitting `needs`
- `runs-on` for `ubuntu-latest`, `windows-latest`, and `macos-latest`
- OS-specific commands and file creation

## Challenges
None encountered in the workflow definitions. If you see YAML syntax errors, validate indentation and the `on` trigger blocks.
\nTest branch update for PR workflow.
