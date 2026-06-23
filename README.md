# asdf-terraformer

[![Build](https://github.com/gr1m0h/asdf-terraformer/actions/workflows/build.yaml/badge.svg)](https://github.com/gr1m0h/asdf-terraformer/actions/workflows/build.yaml)
[![Lint](https://github.com/gr1m0h/asdf-terraformer/actions/workflows/lint.yaml/badge.svg)](https://github.com/gr1m0h/asdf-terraformer/actions/workflows/lint.yaml)

[Terraformer](https://github.com/GoogleCloudPlatform/terraformer) plugin for the [asdf](https://github.com/asdf-vm/asdf) version manager.

## Install

```shell
asdf plugin add terraformer https://github.com/gr1m0h/asdf-terraformer.git
```

Please ensure you also set up the Terraform plugin directory. See the
[Terraformer installation instructions](https://github.com/GoogleCloudPlatform/terraformer#installation),
from Step 4 onwards.

## Usage

See the [asdf documentation](https://asdf-vm.com/manage/core.html) for the full
set of commands. The most common ones are:

```shell
# Show all installable versions
asdf list all terraformer

# Install a specific version
asdf install terraformer latest
asdf install terraformer 0.8.30

# Set a version globally (writes to ~/.tool-versions)
asdf set -u terraformer latest

# Set a version for the current project (writes to ./.tool-versions)
asdf set terraformer 0.8.30
```

## Contributing

Contributions are welcome! This plugin is linted with
[shellcheck](https://www.shellcheck.net/) and
[shfmt](https://github.com/mvdan/sh), and tested with
[asdf-vm/actions](https://github.com/asdf-vm/actions).

The required tooling versions are pinned in [`.tool-versions`](./.tool-versions),
so you can install them with asdf:

```shell
asdf install
```

```shell
# Format the shell scripts
./scripts/format.bash

# Lint the shell scripts
./scripts/lint.bash
```

## License

[MIT](./LICENSE)
