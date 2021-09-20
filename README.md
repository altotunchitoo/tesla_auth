# Tesla Auth

[![CI](https://github.com/adriankumpf/tesla_auth/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/adriankumpf/tesla_auth/actions/workflows/ci.yml)
[![CD](https://github.com/adriankumpf/tesla_auth/actions/workflows/cd.yml/badge.svg?branch=main)](https://github.com/adriankumpf/tesla_auth/actions/workflows/cd.yml)

Securely generate API tokens for third-party access to your Tesla.

Multi-factor authentication (MFA) and Captcha are supported.

## Download

> _Precompiled binaries are currently only available for x86-64._

- [macOS](https://github.com/adriankumpf/tesla_auth/releases/latest/download/tesla-auth-macos.tar.gz)
- [Linux](https://github.com/adriankumpf/tesla_auth/releases/latest/download/tesla-auth-linux.tar.gz)
- [Windows](https://github.com/adriankumpf/tesla_auth/releases/latest/download/tesla-auth-windows.tar.gz)

## Usage

```plain
❯ tesla_auth --help
Usage: tesla_auth [-d]

Tesla API tokens generator

Options:
  -d, --debug       print debug output
  --help            display usage information
```

## Platform-specific dependencies

### macOS

WebKit is native on macOS so **no additional dependencies** are required.

### Windows

WebView2 is powered by Microsoft Edge (Chromium). At the moment it **requires a preview version of Edge** which can be downloaded here: [Microsoft Edge Insider Channels](https://www.microsoftedgeinsider.com/en-us/download)

### Linux

[WebKitGTK](https://webkitgtk.org/) is required for WebView. So please make sure following packages are installed:

#### Arch Linux / Manjaro:

```bash
sudo pacman -S webkit2gtk libappindicator-gtk3
```

#### Debian / Ubuntu:

```bash
sudo apt install libwebkit2gtk-4.0-dev libappindicator3-dev
```

#### Fedora

```bash
sudo dnf install gtk3-devel webkit2gtk3-devel libappindicator-gtk3-devel
```

## License

Apache-2.0/MIT
