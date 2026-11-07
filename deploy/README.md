# openrelik-deploy

##### Obligatory Fine Print

This is not an official Google product (experimental or otherwise), it is just code that happens to be owned by Google.

## Layout and releases

`docker/` holds the production deployment: `docker-compose.yml`, `config.env`
(image versions), `prometheus.yml` and `install.sh`.

On `main`, `config.env` uses the `latest` images; that is what the installer's
"bleeding edge" option installs. A release pins the image versions in
`config.env` on the release commit and tags it `v<version>`. The installer
downloads the compose file, config and the server's `settings_example.toml`
from that tag, so they always belong together. Add the version to `RELEASES`
in `install.sh` on `main` to offer it.

Releases from before the monorepo (0.7.0, 0.6.0) are listed in
`LEGACY_RELEASES` and install from the archived `openrelik-deploy` and
`openrelik-server` repositories, as before.
