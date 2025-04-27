# `fztea-bin`

[`fztea`](https://github.com/jon4hz/fztea) is client for the
[Flipper Zero](https://en.wikipedia.org/wiki/Flipper_Zero) device and serves as
a [TUI](https://en.wikipedia.org/wiki/Text-based_user_interface) alternative to
[qFlipper](https://flipperzero.one/update) (whose [repo](https://github.com/flipperdevices/qFlipper)
is on GitHub), the GUI for to manage the Flipper Zero and update the firmware.
This application can also access the Flipper Zero via remote SSH.

This uses the [Bubble Tea](https://github.com/charmbracelet/bubbletea) TUI
framework from [Charmbracelet](https://charm.sh).

## Maintainer metadata
* [Link](https://github.com/jon4hz/fztea/releases/latest) to latest GH release
* [MPR page](https://mpr.makedeb.org/packages/fztea-bin)
* Architectures: `amd64`, `arm64`
    * Available but not packaged: `armv7`, `i386`(?)
* SHA256 checksums provided for file integrity
* No file authenticity checks (via GPG)

## Maintenance scope

I will maintain this package as long as there isn't an auto-updating method
available for APT-based Linux distributions.
