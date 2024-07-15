# `ente-auth-bin`

This is the desktop client for Ente [Auth](https://ente.io/auth/).

This `PKGBUILD` uses the "trivial" `makedeb` method suggested by Exponential, as
described in [#1](https://github.com/taivlam/aur-mpr-packages/issues/1).

Previously, I tried to make `ente-auth-bin` copy the AUR package for the MPR,
but it turns out that somehow the DEB, which is already in the GH release
assets, is a stand-alone binary - so, this means that the binary can be
"trivially" installed onto the system.

After discussion on the MPR channel on Matrix, `ente-auth-deb` was merged into
`ente-auth-bin`

