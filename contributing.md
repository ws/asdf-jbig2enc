# Contributing

Contributions of any kind are welcome!

## Prerequisites

- [asdf](https://asdf-vm.com) installed
- [shellcheck](https://www.shellcheck.net/) for linting
- [shfmt](https://github.com/mvdan/sh) for formatting

## Testing Locally

Test the plugin by running:

```shell
asdf plugin test jbig2enc https://github.com/ws/asdf-jbig2enc.git "jbig2 --help"
```

To test a specific version:

```shell
asdf plugin test jbig2enc https://github.com/ws/asdf-jbig2enc.git --asdf-tool-version 0.29 "jbig2 --help"
```

To test from a local branch:

```shell
asdf plugin test jbig2enc . --asdf-plugin-gitref HEAD "jbig2 --help"
```

## Linting & Formatting

Run the linter:

```shell
scripts/lint.bash
```

Auto-format code:

```shell
scripts/format.bash
```

## Pull Requests

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Run `scripts/lint.bash` and fix any issues
5. Submit a pull request

Tests run automatically in GitHub Actions on push and PR.
