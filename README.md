[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/hanoii/ddev-drupal-contrib-extras/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/hanoii/ddev-drupal-contrib-extras/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/hanoii/ddev-drupal-contrib-extras)](https://github.com/hanoii/ddev-drupal-contrib-extras/commits)
[![release](https://img.shields.io/github/v/release/hanoii/ddev-drupal-contrib-extras)](https://github.com/hanoii/ddev-drupal-contrib-extras/releases/latest)

# DDEV Drupal Contrib Extras

## Overview

This add-on extends [ddev/ddev-drupal-contrib](https://github.com/ddev/ddev-drupal-contrib) with small extras that are useful for Drupal contrib work but are not yet part of the upstream add-on.

It is meant as a lightweight bridge for practical patches, commands, and tweaks while they are being discussed upstream or are too narrow to maintain there.

## What this adds or fixes

On top of [ddev/ddev-drupal-contrib](https://github.com/ddev/ddev-drupal-contrib), this add-on currently provides:

- Adds `ddev cspell`, which runs Drupal's cspell setup from the web container and supports Yarn PnP. See https://github.com/ddev/ddev-drupal-contrib/pull/55
- Patches `phpcbf` behavior with https://github.com/ddev/ddev-drupal-contrib/pull/175, to ignore `.ddev` paths so code style fixes do not rewrite local DDEV config.

## Installation

```bash
ddev add-on get hanoii/ddev-drupal-contrib-extras
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Credits

[cspell](commands/web/cspell) crafted by [@jameswilson](https://github.com/jameswilson)

**Contributed and maintained by [@hanoii](https://github.com/hanoii)**
