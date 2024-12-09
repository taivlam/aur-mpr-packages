# `electronmail-bin`

## Maintainer metadata
* [MPR page](https://mpr.makedeb.org/packages/electronmail-bin)
* [Link](https://github.com/vladimiry/ElectronMail/releases/latest) to latest GH release
* Only `amd64` architecture
    * For prebuilt binary executables
* SHA256 checksums provided for file integrity
    * Located inside a collapsible `<details>` field in reach GH release description
* No file authenticity method provided (via GPG)

## Background and context
This MPR package is for [ElectronMail](https://github.com/vladimiry/ElectronMail),
a third-party desktop client for Proton Mail that is cross-platform (available
for Windows, macOS, and Linux) and is based on
[Electron](https://en.wikipedia.org/wiki/Electron_(software_framework)).

## Maintaining this MPR package
I will maintain ElectronMail for as long as upstream ElectronMail is maintained.

However, as of February 2024, Proton Tech [officially](https://proton.me/support/mail-desktop-app)
has its own native Proton Mail desktop client in beta for Windows and macOS.

At the rate at which Proton Tech's software engineering moves, I'll still use
ElectronMail, at least until the official Proton Mail desktop client for Linux
is released for APT-based distros via a method that is capable of automatic
updates (more so than the "fancy" way to update via the MPR).

I will keep track of progress on Proton Mail's desktop client for Linux.

## Thanks
Thanks to the prior maintainer, [@hiddeninthesand](https://github.com/hiddeninthesand),
for starting this package.

