I needed [jbig2enc](https://github.com/agl/jbig2enc) for [ocrmypdf](https://github.com/ocrmypdf/OCRmyPDF) ([details](https://ocrmypdf.readthedocs.io/en/latest/jbig2.html)) and decided installing via Homebrew was simply not difficult enough; I wanted to make it a [mise](https://mise.jdx.dev/) package. Since there are no binaries provided by the authors (I think Homebrew is installing from maintainer-managed builds), I followed the [mise docs](https://mise.jdx.dev/dev-tools/backend_architecture.html#use-asdf-plugins-when) directions and created an asdf plugin. This is that plugin!

It was 100% vibe coded, I don't know what I'm doing, you shouldn't use it, etc. etc. I can confirm it works on my specific machine on my specific version of MacOS and absolutely nothing else.

# Dependencies

This plugin builds jbig2enc from source, so you need build tools and libraries installed. Yes we were trying to avoid Brew in the first place, don't ask questions.

**macOS:**

```shell
brew install autoconf automake libtool leptonica
```

# How To Use With Mise

```shell
# Add the plugin
mise plugins install jbig2enc https://github.com/ws/asdf-jbig2enc.git

# Install latest
mise install jbig2enc

# Install a specific version
mise install jbig2enc@0.29

# Set as global default
mise use -g jbig2enc@0.29

# Or set for current directory only
mise use jbig2enc@0.29
```

# How To Use With ocrmypdf

```shell
mise x uv jbig2enc cargo:pngquant -- uvx ocrmypdf yourfile.pdf output.pdf
```