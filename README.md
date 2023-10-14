# restic-deb

Automated Debian packages built directly from official [Restic](https://github.com/restic/restic) release binaries.

## Installation

### via Apt

Install my Debian repository if you haven't already:

```shell
sudo apt-get install ca-certificates curl gnupg
sudo install -m 0755 -d /etc/apt/keyrings
curl -fsSL https://dist.cdzombak.net/deb.key | sudo gpg --dearmor -o /etc/apt/keyrings/dist-cdzombak-net.gpg
sudo chmod 0644 /etc/apt/keyrings/dist-cdzombak-net.gpg
echo -e "deb [signed-by=/etc/apt/keyrings/dist-cdzombak-net.gpg] https://dist.cdzombak.net/deb/3p any 3p\n" | sudo tee -a /etc/apt/sources.list.d/dist-cdzombak-net.list > /dev/null
sudo apt-get update
```

Then install `restic` via `apt-get`:

```shell
sudo apt-get install restic
```

### Manual installation from build artifacts

Debian packages are downloadable from each [GitHub Release](https://github.com/cdzombak/restic-deb/releases).
