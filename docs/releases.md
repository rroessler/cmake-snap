## Release Instructions

Each CMake feature release has its own corresponding branch in this repository.
These branches follow the naming convention `release/X.Y`.
When an official CMake release is made (including release candidates), create or checkout the branch tracking that feature release.
The [GitHub workflow file](.github/workflows/build-snap-packages.yml) must be updated with the appropriate feature release version and publishing track for that branch and version.
The other CMake release version details in that file will determine the version of the snap that is built.
Only tagged releases will upload and publish snaps.
Set the release track to `candidate` for release candidates, or `stable` for regular releases.

CI jobs only publish snap packages to the specified release track.
If publishing for the latest feature release, an extra manual step is required.
The `latest` channel needs to be updated in the [Snapcraft Releases](https://snapcraft.io/cmake/releases) area (login required).
This should be a simple matter of promoting the just-published snaps to the relevant channel (`latest/candidate` or `latest/stable`).
If this is the first regular release after previous release candidates, also close the `latest/candidate` channel after promoting to `latest/stable`.
The candidate channel will then forward to the latest stable release, which ensures anyone tracking the candidate channel moves up to the stable release on their next update.
