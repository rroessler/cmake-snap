<p align="center">
    <a href="https://cmake.org/">
        <img src="https://github.com/rroessler/cmake-snap/blob/master/snap/gui/CMake_Logo.png">
    </a>
    <br />
    <br />
    <b>This is the snap for CMake</b>, a cross-platform, open-source build system generator.
    <br />
    <br />
    <a href="https://snapcraft.io/cmake">
        <img src="https://snapcraft.io/cmake/badge.svg">
    </a>
</p>

## Installation

To install the CMake snap from the Snapcraft store:

```shell
sudo snap install --classic cmake
```

Verify the installation by checking the current version:

```shell
cmake --version
```

> **Note:** Starting with the CMake 3.27 series, snap packages are a wrapper around the official CMake binary releases from Kitware. This currently only includes the `amd64` and `arm64` architectures. For more information see the [documentation on supported architectures](docs/architectures.md).

## Documentation

Access the following documentation for the CMake snap:

- [Release Instructions](docs/releases.md)
- [Supported Architectures](docs/architectures.md)
