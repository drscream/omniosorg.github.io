---
title: Building packages
category: dev
show_in_sidebar: true
---

# Building packages

pkg5 packages are build with a OmniOSce package framework which is developed in
the shell scripting language bash. Packages are provided for two providers:

- [omnios](https://github.com/omniosorg/omnios-build/tree/master/build)
- [extra.omnios](https://github.com/omniosorg/omnios-extra/tree/master/build)

## Building

Before building or contributing a package be sure you've setup and configured
the [build environment](https://omniosce.org/dev/build_instructions). This would
help you to have all repositories stored in `/build`.

### Building existing packages

The `buildctrl` provide you a script to build packages based on the `build.sh`
package description files.

```
$ cd /build/omnios-build/build
$ ./buildctrl build PROG
```

The `PROG` will be build and a package should be provided into `$PKGSRVR`
(default: `file:///build/repo`).

## Developing

### File structure

- `build/`: package scripts and building tools
  - `$PROG/build.sh`: build script
  - `$PROG/files/`: folder for additional files to install
  - `$PROG/local.mog`: transmogrify script
  - `$PROG/patches`: folder for additional patches
- `doc`: package and release information, documentation
- `lib`: library and configuration for building tools

### `build.sh` structure



### `local.mog` structure

## Contributing
