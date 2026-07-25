[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/ptmkenny/ddev-claude-code/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/ptmkenny/ddev-claude-code/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/ptmkenny/ddev-claude-code)](https://github.com/ptmkenny/ddev-claude-code/commits)
[![release](https://img.shields.io/github/v/release/ptmkenny/ddev-claude-code)](https://github.com/ptmkenny/ddev-claude-code/releases/latest)

# DDEV Claude Code

## Overview

This add-on integrates Claude Code into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get ptmkenny/ddev-claude-code
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Claude Code |
| `ddev logs -s claude-code` | Check Claude Code logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.claude-code --claude-code-docker-image="ddev/ddev-utilities:latest"
ddev add-on get ptmkenny/ddev-claude-code
ddev restart
```

Make sure to commit the `.ddev/.env.claude-code` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `CLAUDE_CODE_DOCKER_IMAGE` | `--claude-code-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@ptmkenny](https://github.com/ptmkenny)**
