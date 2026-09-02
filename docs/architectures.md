## Supported Architectures

Starting with the CMake 3.27 release series, snap packages are essentially just a wrapper around the official CMake binary releases from Kitware.
Snap packages are only provided for the architectures that have an official Kitware release.
Currently, that is only `amd64` and `arm64` (Kitware releases call these `x86_64` and `aarch64` respectively).
For CMake 3.27 onward, these will be the only architectures for which new snap packages will be created.

For CMake 3.26 and earlier, snap packages were built using the snapcraft remote build service for architectures `amd64`, `arm64`, `armhf`, `ppc64el`, `s390x` and `i386`.
These snaps had some differences to the official packages, mostly due to the way Qt was built and incorporated into the snap building process.
These older snaps will continue to be available for all architectures, but `armhf`, `ppc64el`, `s390x` and `i386` will not receive any updates for CMake 3.27 and later.
