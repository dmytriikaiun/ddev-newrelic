[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/dmytriikaiun/ddev-newrelic/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/dmytriikaiun/ddev-newrelic/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/dmytriikaiun/ddev-newrelic)](https://github.com/dmytriikaiun/ddev-newrelic/commits)
[![release](https://img.shields.io/github/v/release/dmytriikaiun/ddev-newrelic)](https://github.com/dmytriikaiun/ddev-newrelic/releases/latest)

# DDEV Newrelic

## Overview

This add-on integrates Newrelic into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get dmytriikaiun/ddev-newrelic
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Newrelic |
| `ddev logs -s newrelic` | Check Newrelic logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.newrelic --newrelic-docker-image="ddev/ddev-utilities:latest"
ddev add-on get dmytriikaiun/ddev-newrelic
ddev restart
```

Make sure to commit the `.ddev/.env.newrelic` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `NEWRELIC_DOCKER_IMAGE` | `--newrelic-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@dmytriikaiun](https://github.com/dmytriikaiun)**
