# [`mouse-configurator`](https://aur.archlinux.org/packages/mouse-configurator)

An AUR package for [Mouse Configurator](https://github.com/pop-os/mouse-configurator),
originally created by [System76](https://system76.com/) for the
[HP 935 Creator Wireless Mouse](https://www.hp.com/us-en/shop/pdp/hp-935-creator-wireless-mouse).

## Notes
* There seems to be some informational/warning messages when some Cargo crates are built.
* This makes sense, as the latest release was from [June 2022](https://github.com/pop-os/mouse-configurator/releases/tag/v1.0.0).
    * Some of the underlying code will likely need change as Rust updates.

## Historical context
This custom Pop!\_OS package was created alongside the release of the HP Dev One
[laptop](https://en.wikipedia.org/wiki/HP_EliteBook#HP_Dev_One) in 2022.  The
mouse mentioned above was being sold as an accessory, along with the System76
[Launch Configurable Keyboard](https://system76.com/accessories/launch).

## Thanks
* [Aaron Honeycut](https://ahoneybun.net/), Happiness Architect at System76
    * I basically copied and pasted the PKGBUILD for System76 Launch Keyboard (`system76-keyboard-configurator` on the [AUR](https://aur.archlinux.org/packages/system76-keyboard-configurator))
