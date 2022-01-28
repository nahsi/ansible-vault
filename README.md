# Vault

Install, configure and maintain [Vault](https://www.vaultproject.io) - a tool
for managing secrets from HashiCorp.

## Role Variables

See [defaults/](defaults/) for details and examples.

#### `vault_version`

- version to use

#### `vault_dirs`

- a map of directories to create

#### `vault_config`

- main [configuration](https://www.vaultproject.io/docs/configuration) file

#### `vault_configs`

- map of configuration files to create in `config.d` directory. Restart on
  changes

#### `vault_user`

- owner of vault process and files

#### `vault_grop`

- group of `vault_user`

#### `vault_download_url`

- url to get vault archive from

#### `vault_service`

- openrc service file

#### `vault_unitfile`

- systemd unit file

#### `skip_handlers`

- skipt vault restart/reload - useful when building images with Packer

## Tags

- `config` - update vault unit/service file and sync configuration files

## Author

- **Anatoly Laskaris** - [nahsi](https://github.com/nahsi)
