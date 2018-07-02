---
layout: page
title: Packaging
---

## Not tagging updated package versions

Package developers usually work on cutting-edge branches of their packages, and often forget that the standard user will run `add package` to download the last tagged version by default. This tagged version should be kept up-to-date with bug fixes and new features.

### Anti-pattern

Pushing an important bug fix to a package repository without tagging an updated version in METADATA.

### Best practice

Tag packages regularly using [semantic versioning](https://semver.org) and push the updates to Julia's METADATA repository. [Attobot](https://github.com/attobot/attobot) makes this process easier.
