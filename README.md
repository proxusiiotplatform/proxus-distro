# Proxus Industrial Data Platform: downloads

This repository is where Proxus publishes its installation packages. It holds no source code.

Download a package from [Releases](../../releases). Each release is one Proxus version and carries a
`SHA256SUMS` file; check every file against it before you install.

| Package | Files in a release | Guide |
| --- | --- | --- |
| Docker Compose (Linux, Windows, macOS) | `docker-compose.yml`, `docker-compose.keycloak.yml`, `proxus-realm.json` (used by the installer), and `proxus-docker_<version>.zip` with the installers for hosts without internet access | [Install](https://proxus.io/docs/get-started/install) |
| Siemens Industrial Edge app, x86-64 | `proxus-industrial-edge_<version>_amd64.app.zip` | [Siemens Industrial Edge](https://proxus.io/docs/operate/siemens-industrial-edge) |
| Siemens Industrial Edge app, arm64 | `proxus-industrial-edge_<version>_arm64.app.zip` | [Siemens Industrial Edge](https://proxus.io/docs/operate/siemens-industrial-edge) |

Install, update and back up with the installer: `curl -fsSL https://proxus.io/install.sh | bash` on Linux and macOS,
`irm https://proxus.io/install.ps1 | iex` on Windows. It takes the files of the latest release from here and checks
them against `SHA256SUMS.txt`.

The container images are on Docker Hub (`proxusplatform/proxus-server`, `proxusplatform/proxus-ui`). Each release's
`docker-compose.yml` uses the images of that release. See [Docker](https://proxus.io/docs/operate/docker).

The latest version of a file is always at
`https://github.com/proxusiiotplatform/proxus-distro/releases/latest/download/<file>`.

Proxus needs a license key. See [License](https://proxus.io/docs/administer/license). For help, contact
Proxus support through [proxus.io](https://proxus.io).
