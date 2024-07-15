# `ente-desktop-bin`

This MPR [package](https://mpr.makedeb.org/packages/ente-auth-bin) is for ente
Auth Desktop, the desktop client for [ente Auth](https://github.com/ente-io/ente/tree/main/auth).
(ente is using a monorepo structure, and ente Auth is a subdirectory within this
repo, which originally was for [ente Photos](https://github.com/ente-io/ente).)

ente Auth's desktop client was released in [v2.50.0](https://github.com/ente-io/ente/releases/tag/auth-v2.0.50)
on March 29, 2024.  After using ente Auth on Android and determining that having
[E2EE](https://en.wikipedia.org/wiki/End-to-end_encryption) cloud backups of my
[2FA](https://en.wikipedia.org/wiki/Multi-factor_authentication)
[TOTP](https://en.wikipedia.org/wiki/Time-based_one-time_password) codes would
be useful to me, I decided to package ente Auth Desktop for the MPR for
[v2.0.54](https://github.com/ente-io/ente/releases/tag/auth-v2.0.54) and onward.

## How long I will maintain this package

I will maintain this package as long as there isn't a third-party 
[APT](https://en.wikipedia.org/wiki/APT_(software)) repo that will self-update
the ente Auth Desktop client on Debian/Ubuntu.  Any method that's more robust
than manually downloading a [`.deb`](https://en.wikipedia.org/wiki/Deb_(file_format))
archive and installing it with [`gdebi`](https://launchpad.net/gdebi/) -- i.e.,
using:
```
$ sudo gdebi <package-name>.deb
```

## Thanks

Thanks to Alessandro Bernardello for the `ente-auth-bin` package on the
[AUR](https://aur.archlinux.org/packages/ente-auth-bin); and the immediate past
maintainer [@hiddeninthesand](https://github.com/hiddeninthesand) for both
`freetube-bin` and `electronmail-bin` (especially the latter) on the MPR (for
showing how to use no install scripts for plain `.deb` archives).

I was able to "map" most of the Arch Linux dependencies into the Debian/Ubuntu
equivalents.

