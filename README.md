<div align="center">

# asdf-jbig2enc [![Build](https://github.com/ws/asdf-jbig2enc/actions/workflows/build.yml/badge.svg)](https://github.com/ws/asdf-jbig2enc/actions/workflows/build.yml) [![Lint](https://github.com/ws/asdf-jbig2enc/actions/workflows/lint.yml/badge.svg)](https://github.com/ws/asdf-jbig2enc/actions/workflows/lint.yml)

[jbig2enc](https://github.com/agl/jbig2enc) plugin for the [asdf version manager](https://asdf-vm.com).

</div>

# Contents

- [Dependencies](#dependencies)
- [Install](#install)
- [Contributing](#contributing)
- [License](#license)

# Dependencies

**TODO: adapt this section**

- `bash`, `curl`, `tar`, and [POSIX utilities](https://pubs.opengroup.org/onlinepubs/9699919799/idx/utilities.html).
- `SOME_ENV_VAR`: set this environment variable in your shell config to load the correct version of tool x.

# Install

Plugin:

```shell
asdf plugin add jbig2enc
# or
asdf plugin add jbig2enc https://github.com/ws/asdf-jbig2enc.git
```

jbig2enc:

```shell
# Show all installable versions
asdf list-all jbig2enc

# Install specific version
asdf install jbig2enc latest

# Set a version globally (on your ~/.tool-versions file)
asdf global jbig2enc latest

# Now jbig2enc commands are available
jbig2enc --version
```

Check [asdf](https://github.com/asdf-vm/asdf) readme for more instructions on how to
install & manage versions.

# Contributing

Contributions of any kind welcome! See the [contributing guide](contributing.md).

[Thanks goes to these contributors](https://github.com/ws/asdf-jbig2enc/graphs/contributors)!

# License

See [LICENSE](LICENSE) © [Will Smidlein](https://github.com/ws/)
