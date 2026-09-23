# vst-bench public resources

Public source downloads, documentation, and issue reporting for `vst-bench-ml`
and `vst-bench-dataset-host`.

## Source downloads and citation

Version 0.1.0 was published on 23 September 2026. Download each source ZIP from
its Zenodo record and cite the version-specific DOI.

| Software | Source archive | DOI |
| --- | --- | --- |
| vst-bench-ml | [Zenodo record](https://zenodo.org/records/22924036) | [10.5281/zenodo.22924036](https://doi.org/10.5281/zenodo.22924036) |
| vst-bench-dataset-host | [Zenodo record](https://zenodo.org/records/22924073) | [10.5281/zenodo.22924073](https://doi.org/10.5281/zenodo.22924073) |

`vst-bench-ml` samples audio-plugin parameters, coordinates rendering through a
separately installed localhost host, records outputs and failed/dropped attempts,
and verifies sealed dataset integrity offline. The companion archive supplies a
self-authored, sample-free VST3 test instrument, offline runner, JSON-RPC host,
and validation scripts.

This repository is the public documentation and support entry point, not a clone
of the development repositories. The versioned software source is in the Zenodo
ZIPs; private repository access is not required. No development history, private
research material, datasets, generated audio, plugin binaries, or SDK source is
included here.

## Getting started

1. Download both source ZIPs from Zenodo.
2. Check their SHA-256 values against [CHECKSUMS.sha256](CHECKSUMS.sha256), then
   unpack them into separate directories.
3. Follow the host archive's `README.md` for the native build, locked Python
   environment, and complete validation workflow.

The demonstrated setup is macOS arm64 with Python 3.12.13. Building requires a
C++17 compiler, CMake 3.25 or newer, and Git/network access for the separately
retrieved pinned VST3 SDK. Keep builds, environments, caches, and results outside
the source roots. The source manifests reject missing, changed, or extra files.

Integrity and repeatability on this setup do not establish cross-platform
compatibility, scientific suitability, or perceptual quality.

## Questions, bugs, and contributions

Use [GitHub Issues](https://github.com/itsuzef/vst-bench-public/issues) for public
questions, bug reports, and proposed improvements. Include the affected archive
version, operating system, Python version, command, and a minimal reproducible
example using the sample-free fixture where possible. Remove secrets, personal
data, private paths, proprietary assets, and unlicensed audio before posting.

Documentation corrections can be proposed as pull requests here. For source
changes, open an issue describing the proposed change and a minimal patch against
the published snapshot. See [CONTRIBUTING.md](CONTRIBUTING.md). No response-time
or ongoing-support guarantee is made.

## Licences

The software source and this repository's documentation use the MIT licence.
The companion's `OUTPUT-LICENSE` dedicates only qualifying sample-free generated
fixture outputs under CC0-1.0. It does not relicense source code, external SDKs,
plugins, or other audio. Consult each archive's `LICENSE`, `OUTPUT-LICENSE` where
applicable, and `THIRD_PARTY.md` for the boundaries.

See [CHANGELOG.md](CHANGELOG.md) for the documentation correction to the host
archive and its checksum history.
