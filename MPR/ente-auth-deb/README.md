# `ente-auth-deb`

This `PKGBUILD` uses the "trivial" `makedeb` method suggested by Exponential, as
described in #1.

Previously, I tried to make `ente-auth-bin` copy the AUR package for the MPR,
but it turns out that somehow the DEB, which is already in the GH release
assets, is a stand-alone binary - so, this means that the binary can be
"trivially" installed onto the system.

A merge request will be made to join `ente-auth-bin` into `ente-auth-deb`.

