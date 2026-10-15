# cerbero-deps

This repository serves as an **additional source mirror** for [Cerbero](https://gitlab.freedesktop.org/gstreamer/cerbero) projects maintained by **Fluendo**.

## Usage

To use this repository as an extra mirror in your Cerbero build configuration, add the following line to your `cerbero/config/cerbero.cbc` file:

```python
extra_mirrors = ["https://fluendo.github.io/cerbero-deps"]
````

This enables Cerbero to fetch prebuilt source hosted here when building packages.

Example [at gst.wasm](https://github.com/fluendo/gst.wasm/commit/a87c83298e0098136d780f41bdf1a79ecc0aa9ff)

## Repository Maintenance

* **Source tarballs** must be added to the repository manually via commits or pull requests.
* After adding binaries, **GitHub Pages** must be updated manually to reflect the changes.
* This repository is served via GitHub Pages at:
  [https://fluendo.github.io/cerbero-deps](https://fluendo.github.io/cerbero-deps)

## Notes

* Only use this repository for hosting trusted dependencies.
* Ensure that file structure and naming conventions are compatible with Cerbero’s expectations.

## License

This repository contains only source files used by Cerbero; each file may be subject to its own license. Please verify individual components before redistribution.

