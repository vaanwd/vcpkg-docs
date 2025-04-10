---
title: Glossary of vcpkg terms
description: This article provides a glossary of common terms-of-art used in vcpkg's documentation.
author: vicroms
ms.author: viromer
ms.date: 01/10/2024
ms.topic: glossary
---

# Glossary: vcpkg

Some of the terms used in this documentation have similar meanings when
discussed by the community. Because of that, and to avoid confusion and
ambiguity this article provides specific meanings for these terms.

## A

### Asset

An artifact that needs to be downloaded typically from the Internet and made
available locally, often the input of a build process. Assets include source
code archives, pre-built binaries, or other files that are required to build
a package.

## B

### Binary package

The installation output produced by vcpkg packaged into a restorable format.
Binary packages hold the build-output of a package (binaries, build system
integration files, usage documentation, license, and other files).

### Build artifact

Files created during the build process, essentially the output of your build
process. Artifacts include libraries, executables, headers, logs, and other
files that are generated by compiling the source code.

## C

### Classic Mode

A mode of operation that installs packages into a shared tree.

See [classic mode documentation](../concepts/classic-mode.md) to learn more.

## L

### Library

A piece of software (source code, binary files, documentation, license, etc.)
that is intended to be reused by other software. Most ports in the [vcpkg
registry](<https://github.com/Microsoft/vcpkg>) install C/C++ libraries.

## M

### Manifest

A file named [`vcpkg.json`](../reference/vcpkg-json.md) that describes the
metadata, such as dependencies, of a port or a project.

See the [manifests documentation](../concepts/manifest-mode.md) to learn more.

## O

### Overlay port/triplet

A locally available port or triplet. Usually used to provide a port or triplet
that is not part of a registry, or to override the name of a port or triplet in
a registry.

See the [overlays documentation](../concepts/overlay-ports.md) to learn more.

## P

### Package

A package can contain a library, collection of libraries, build scripts,
software tools, or other components necessary for their use. The goal of vcpkg
is to install these packages [available during your projects
builds](../concepts/build-system-integration.md).

### Package manager

A package manager is a tool that manages dependencies for a project by
offering features to install, upgrade, and integrate software libraries and
tools. Package managers help you find, install, and update the libraries and
tools that your project needs, and handle the compatibility and configuration
issues that may arise.

### Patch

A set of code changes/diffs applied to a source code project before building.
These changes are usually not integrated into the latest upstream release.
Patches are used to fix bugs, add features, or customize the behavior of a package.

### Port

A vcpkg-specific term, a port contains:

* Metadata about a [package](#package): name, version, dependencies, supported features,
  etc.
* Instructions to acquire, build if necessary, and install the package.

See the [ports documentation](../concepts/ports.md) to learn more.

## R

### Registry

A vcpkg-specific term, a registry is a collection of [ports](#port) available to install in vcpkg.  Registries follow a specific
structure described in the [registries documentation](../concepts/registries.md).

vcpkg offers a curated registry available at <https://github.com/Microsoft/vcpkg>, and users can create their own [custom
registries](../produce/publish-to-a-git-registry.md) to host their own collection of ports.

## S

### System Package Manager

A package manager such as apt-get designed to be used with a particular
platform such as Linux, or brew for MacOS. System package managers install
packages and libraries system wide, rather than for a particular project.

## T

### Triplet

A set of properties or script used to describe a target or host environment,
which affects how vcpkg builds a library. The triplet specifies linkage
type, build flags, and other options that affect how a package is built and installed.

See [triplet documentation](../concepts/triplets.md) to learn more.

## U

### Upstream

Refers to the repository where the source code changes for a project originates
from. Upstream is usually the original or official source of a project, where
the main development takes place. Upstream may also refer to the maintainers
or authors of a project.
