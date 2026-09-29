# vst-bench public resources

Public source downloads, documentation, and issue reporting for `vst-bench-ml`
and `vst-bench-dataset-host`.

## Current software and documentation

The maintained source repositories provide line-level history, installation
instructions, user guides, and issue reporting:

- [vst-bench-ml](https://github.com/itsuzef/vst-bench-ml-public): Python package.
- [vst-bench-dataset-host](https://github.com/itsuzef/vst-bench-dataset-host-public):
  sample-free fixture, native host, and full validation workflow.
- [User guide](https://github.com/itsuzef/vst-bench-ml-public/blob/main/docs/README.md).
- [First dataset walkthrough](https://github.com/itsuzef/vst-bench-dataset-host-public/blob/main/docs/QUICKSTART.md).
- [PyPI](https://pypi.org/project/vst-bench-ml/): `python -m pip install vst-bench-ml==0.1.1`.

This page retains the original archive records and checksum history. The new public
histories start with documented imports of those source snapshots. Earlier private
development history is not included.

## Historical 0.1.0 source downloads and citation

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

## Getting started

Use the current package installation guide and companion walkthrough linked above.
To reproduce the historical 0.1.0 release, download the two ZIPs, check their
SHA-256 values against [CHECKSUMS.sha256](CHECKSUMS.sha256), and follow the host
archive's README. Keep extracted archives intact and build outside them.

The demonstrated rendering environment is macOS arm64 and Python 3.12. Building
the companion requires C++17, CMake 3.25+, and the separately retrieved pinned VST3
SDK. Integrity and repeatability on a tested setup do not establish general
portability, scientific suitability, or perceptual quality.

## Questions, bugs, and contributions

Use [GitHub Issues](https://github.com/itsuzef/vst-bench-public/issues) for public
questions, bug reports, and proposed improvements. Include the affected archive
version, operating system, Python version, command, and a minimal reproducible
example using the sample-free fixture where possible. Remove secrets, personal
data, private paths, proprietary assets, and unlicensed audio before posting.

Documentation corrections to this page can be proposed here. Submit software
changes and software-specific issues to the corresponding public source repository.
See [CONTRIBUTING.md](CONTRIBUTING.md). No response-time or ongoing-support guarantee
is made.

## Licences

The software source and this repository's documentation use the MIT licence.
The companion's `OUTPUT-LICENSE` dedicates only qualifying sample-free generated
fixture outputs under CC0-1.0. It does not relicense source code, external SDKs,
plugins, or other audio. Consult each archive's `LICENSE`, `OUTPUT-LICENSE` where
applicable, and `THIRD_PARTY.md` for the boundaries.

See [CHANGELOG.md](CHANGELOG.md) for the documentation correction to the host
archive and its checksum history.
