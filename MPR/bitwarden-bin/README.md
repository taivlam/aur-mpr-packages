# `bitwarden-bin`

## Maintainer metadata
* Architectures: `amd64` only for prebuilt binary executables
* SHA512 checksums (in base 64) generated in YAML files
    * So, SHA512 is default upstream checksum
    * Use the following one-line command to verify checksum:
      ```
      $ sha512sum <latest-binary-name>.deb | cut -f1 -d\  | xxd -r -p | base64 -w0
      ```
* SHA256 checksums also generated
* No authenticity checks (via GPG tools)
* Latest release on [GitHub](https://github.com/bitwarden/clients/releases](https://github.com/bitwarden/clients/releases?q=desktop&expanded=true)
    * This is a mono-repo also for the Web and CLI clients
    * So, search for desktop releases
    * In general, manually check for new latest release for desktop
* [MPR page](https://mpr.makedeb.org/packages/bitwarden-bin)

## Contect and background
This MPR [package](https://mpr.makedeb.org/packages/bitwarden-bin) is for the
[Bitwarden](https://en.wikipedia.org/wiki/Bitwarden) desktop client for Linux
distros based on [APT](https://en.wikipedia.org/wiki/APT_(software)) (i.e.,
Debian/Ubuntu).

## Notes
* Official `.deb` archive from Bitwarden's official download [page](https://bitwarden.com/download/) lack auto-updates
* For the foreseeable future, I will maintain this package as long as Bitwarden's APT-based client doesn't auto-update

## Thanks
Thanks to the prior maintainer, Hunter Wittenborn ([@hwittenborn](https://github.com/hwittenborn)),
who is the lead developer of [makedeb](https://www.makedeb.org/) and the [MPR](https://mpr.makedeb.org/),
for starting this package.

