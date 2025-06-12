# `simplex-desktop-bin`

## Maintainer metadata

* Platform: `amd64` only
* Integrity check: SHA256 (through CI) and SHA512 checksums provided
* Authenticity check: not yet for DEB binaries
    * Detacted GPG signatures for SHA 256 checksums, but only for Ubuntu server tarballs
        * Will keep watch to see if more builds are added
    * GPG keys from SimpleX team and Flux team (the latter provides servers for SimpleX services)
    * Since [v6.3.2](https://github.com/simplex-chat/simplex-chat/releases/tag/v6.3.2)
* [Link](https://github.com/simplex-chat/simplex-chat/releases/latest) to latest GH release
* MPR package [page](https://mpr.makedeb.org/packages/simplex-desktop-bin)

## Context and background info

[SimpleX Chat](https://simplex.chat/) (or SimpleX, for short) is a newer E2EE
communication application that has no user identifiers.

The project offers a desktop client.

I am currently not sure how to explain how the Debian-/Ubuntu-based installation
options work.  Besides the AppImage for Linux, there is a pair of releases that
end with either `*-ubuntu-20_04-x86_64` or `*-ubuntu-22_04-x86_64`,
respectively.  I presume these are some sort of `*.tar.gz`-style archives.
However, I haven't looked into these archives that are created with each GH
release, as there are precompiled DEB archives that end with
`*-ubuntu-20_04-x86_64.deb` or `*-ubuntu-22_04-x86_64.deb`, respectively.

The splitting of version between Ubuntu 20.04 LTS or older and 22.04 LTS or
newer are likely related to this GH issue: simplex-chat/simplex-chat#1274.

Since I am testing on essentially Ubuntu 24.04 LTS, according to the MPR
[support policy](https://docs.makedeb.org/using-the-mpr/support-policy/), I will
only be using the version of SimpleX for Ubuntu 22.04 LTS or later.

### Maintenance scope

I will maintain this package until the project offers an option that allows
DEB archives to auto-update.
