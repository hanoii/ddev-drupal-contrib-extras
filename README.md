[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/hanoii/ddev-drupal-contrib-extras/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/hanoii/ddev-drupal-contrib-extras/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/hanoii/ddev-drupal-contrib-extras)](https://github.com/hanoii/ddev-drupal-contrib-extras/commits)
[![release](https://img.shields.io/github/v/release/hanoii/ddev-drupal-contrib-extras)](https://github.com/hanoii/ddev-drupal-contrib-extras/releases/latest)

# DDEV Drupal Contrib Extras

## Overview

This add-on integrates Drupal Contrib Extras into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get hanoii/ddev-drupal-contrib-extras
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Drupal Contrib Extras |
| `ddev logs -s drupal-contrib-extras` | Check Drupal Contrib Extras logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.drupal-contrib-extras --drupal-contrib-extras-docker-image="ddev/ddev-utilities:latest"
ddev add-on get hanoii/ddev-drupal-contrib-extras
ddev restart
```

Make sure to commit the `.ddev/.env.drupal-contrib-extras` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `DRUPAL_CONTRIB_EXTRAS_DOCKER_IMAGE` | `--drupal-contrib-extras-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@hanoii](https://github.com/hanoii)**
