# Contributing

Testing Locally:

```shell
asdf plugin test <plugin-name> <plugin-url> [--asdf-tool-version <version>] [--asdf-plugin-gitref <git-ref>] [test-command*]

# TODO: adapt this
asdf plugin test jbig2enc https://github.com/ws/asdf-jbig2enc.git "jbig2enc --version"
```

Tests are automatically run in GitHub Actions on push and PR.
