---
docid: getting-started
title: Getting started with Infer
layout: docs
permalink: /docs/getting-started.html
---

## Get Infer

You can use Homebrew (Mac only), our binary releases, build infer from
source, or use our Docker image.

On Mac (Mojave), the simplest way is to use [Homebrew](http://brew.sh/). There is a user-provided tap for infer. Type this into a terminal:

```sh
brew install amar1729/infer/infer
```

For Mac pre-Mojave, use Homebrew core:

```sh
brew install infer
```

On Linux, or if you do not wish to use Homebrew on Mac, use our
latest [binary
release](https://github.com/facebook/infer/releases/latest). Download
the tarball then extract it anywhere on your system to start using
infer. For example, this downloads infer in /opt on Linux (replace
`VERSION` with the latest release, eg `VERSION=0.17.0`):

```sh
VERSION=0.XX.Y; \
curl -sSL "https://github.com/facebook/infer/releases/download/v$VERSION/infer-linux64-v$VERSION.tar.xz" \
| sudo tar -C /opt -xJ && \
ln -s "/opt/infer-linux64-v$VERSION/bin/infer" /usr/local/bin/infer
```

If the binaries do not work for you, or if you would rather build
infer from source, follow the [install from
source](https://github.com/facebook/infer/blob/master/INSTALL.md#install-infer-from-source)
instructions to install Infer on your system.

Alternatively, use our
[Docker](https://docs.docker.com/engine/installation/) image:

```sh
wget -O Dockerfile https://raw.githubusercontent.com/facebook/infer/master/docker/0.14.0/Dockerfile
wget -O run.sh https://raw.githubusercontent.com/facebook/infer/master/docker/0.14.0/run.sh
sh run.sh
```

## Try Infer in your browser

Try Infer on a small example on [Codeboard](https://codeboard.io/projects/11587?view=2.1-21.0-22.0).