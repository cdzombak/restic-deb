# restic-deb

Automated Debian packages built directly from official [Restic](https://github.com/restic/restic) release binaries.

## Installation

### via PackageCloud

Install my PackageCloud Debian repository if you haven't already:
```shell
curl -s https://packagecloud.io/install/repositories/cdzombak/3p/script.deb.sh?any=true | sudo bash
```

Then install `restic` via `apt-get`:
```shell
sudo apt-get install restic
```

### Manual installation from build artifacts

Debian packages are downloadable from each [GitHub Release](https://github.com/cdzombak/restic-deb/releases).
