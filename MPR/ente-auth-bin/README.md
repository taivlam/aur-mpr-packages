# `ente-auth-bin`
## Maintainer metadata
* Only `amd64` for architecture
* [Repo](https://github.com/ente-io/ente/tree/main/auth) for Auth is nested inside the general repo for Ente
    * However, [releases](https://github.com/ente-io/ente/releases) are in a monorepo for both Ente Auth (desktop and mobile) and all Photos components (except the Photos desktop client)
* SHA256 checksums given for integrity verification
    * But no authenticity checks (via GPG tools)
* [MPR page](https://mpr.makedeb.org/packages/ente-auth-bin)

## Context and background
This is the desktop client for Ente [Auth](https://ente.io/auth/).

This `PKGBUILD` uses the "trivial" `makedeb` method suggested by Exponential, as
described in [#1](https://github.com/taivlam/aur-mpr-packages/issues/1).

Previously, I tried to make `ente-auth-bin` copy the AUR package for the MPR,
but it turns out that somehow the DEB, which is already in the GH release
assets, is a stand-alone binary - so, this means that the binary can be
"trivially" installed onto the system.

After discussion on the MPR channel on Matrix, `ente-auth-deb` was merged into
`ente-auth-bin`
