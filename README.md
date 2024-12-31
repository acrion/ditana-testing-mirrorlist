# ditana-testing-mirrorlist

This package provides a testing mirrorlist for Ditana GNU/Linux, used for development and testing purposes.

## Description

`ditana-testing-mirrorlist` contains a list of mirror servers that host testing versions of Ditana packages. This mirrorlist is crucial for developers and testers who need to validate changes to Arch packages before they are integrated into the main Ditana distribution.

## Purpose

The primary purpose of this package is to facilitate a special mode in the Ditana ISO creation process. When this mode is activated, the ISO creation script references this testing mirrorlist instead of the standard one. This allows for:

1. Testing of modified Arch packages
2. Validation of changes before integration into the main distribution
3. Creation of specialized ISO images for development and testing purposes

## Usage

This mirrorlist is not intended for regular users. It’s primarily used by:

1. Ditana developers
2. Package maintainers
3. Testers working on new features or bug fixes

To use this mirrorlist in the ISO creation process:

1. Copy the modified packages to the server specified in the testing mirrorlist
2. Activate the special mode in the ISO creation script
3. Create the ISO image

The resulting ISO will use the packages from the testing mirrors, allowing for thorough testing of changes.

## Installation

This package is not installed by default. For development installations:

```bash
sudo pacman -S ditana-testing-mirrorlist
```

## Configuration

The mirrorlist is installed to:

```
/etc/pacman.d/ditana-testing-mirrorlist
```

To use this mirrorlist, you need to modify your pacman configuration or use it explicitly in your development processes.

## Note

Using this testing mirrorlist in a production environment is not recommended, as it may contain unstable or experimental packages.

For more information about Ditana GNU/Linux development, visit [https://ditana.org](https://ditana.org)
