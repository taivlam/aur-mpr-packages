# `mudita-center-appimage`

This AUR package uses the [AppImage](https://en.wikipedia.org/wiki/AppImage)
version the application, as this is the only binary file available for Mudita
Center from [GitHub](https://github.com/mudita/mudita-center).

This is the first AUR package I adopted.

## Change these items after every upstream update
* `pkgver`
* `pkgrel` (if needed)
* `sha256sums_x86_64`

Lastly make sure to run:
```
$ makepkg --printsrcinfo > .SRCINFO
```
to keep the `.SRCINFO` up-to-date!

This is here to help me remember what changes to the `PKGBUILD` I need to make.
I will keep reading the [AUR submission guidelines](https://wiki.archlinux.org/title/AUR_submission_guidelines)
to make sure everything is proper.

## Background info

[Mudita](https://mudita.com/) is a Polish technology company that started off
making an e-ink cell phone called the [Mudita Pure](https://mudita.com/products/phones/mudita-pure/).
The Mudita Pure first started via a Kickstarter crowdfunding
[campaign](https://www.kickstarter.com/projects/mudita/mudita-pure-your-minimalist-phone)
in 2019 and continued with an in-demand Indiegogo
[campaign](https://www.indiegogo.com/projects/mudita-pure-your-minimalist-phone#/).

Mudita Pure's operating system is [MuditaOS](https://mudita.com/products/phones/mudita-pure/muditaos/)
and the source code is on [GitHub](https://github.com/mudita/MuditaOS).

[Mudita Center](https://mudita.com/products/software-apps/mudita-center/) is a
desktop application that lets users update Mudita Pure devices via a USB
connection.  This is the only way to update MuditaOS, even when Mudita Pure is
being used as a mobile Wi-Fi hotspot.

