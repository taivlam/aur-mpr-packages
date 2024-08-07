# `bitwarden-bin`

This MPR [package](https://mpr.makedeb.org/packages/bitwarden-bin) is for the
[Bitwarden](https://en.wikipedia.org/wiki/Bitwarden) desktop client for Linux
distros based on [APT](https://en.wikipedia.org/wiki/APT_(software)) (i.e.,
Debian/Ubuntu).

## Latest release
* On [GitHub](https://github.com/bitwarden/clients/releases)
    * This is a mono-repo also for the Web and CLI clients

## Notes
* Official `.deb` archive from Bitwarden's official download [page](https://bitwarden.com/download/) lack auto-updates
* For the foreseeable future, I will maintain this package as long as Bitwarden's APT-based client doesn't auto-update
* Use SHA256 checksums
    * These are published by Bitwarden for every production release in `sha256-checksums.txt`

## Thanks
Thanks to the prior maintainer, Hunter Wittenborn ([@hwittenborn](https://github.com/hwittenborn)),
who is the lead developer of [makedeb](https://www.makedeb.org/) and the [MPR](https://mpr.makedeb.org/),
for starting this package.

