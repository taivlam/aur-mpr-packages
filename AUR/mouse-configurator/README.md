# `mouse-configurator`

* This AUR package is for [Mouse Configurator](https://github.com/pop-os/mouse-configurator), originally created by [System76](https://system76.com/) for the [HP 935 Creator Wireless Mouse](https://www.hp.com/us-en/shop/pdp/hp-935-creator-wireless-mouse).
    * From what I can tell, the [HP 975 Dual-Mode Wireless Keyboard](https://www.hp.com/us-en/shop/pdp/hp-975-dual-mode-wireless-keyboard-p-3z726aa-aba-1) is the black programmable wireless keyboard that matches the black of the 935 wireless mouse.
    * Currently there is no bundle with the 975 wireless keyboard and the 935 wireless mouse.
* Also this application works with the [HP 930 Creator Wirless Mouse](https://www.hp.com/us-en/shop/pdp/hp-silver-930-creator-wireless-mouse).
    * This mouse is [bundled](https://www.hp.com/us-en/shop/pdp/hp-programmable-wireless-keyboard-wireless-creator-mouse-bundle-970-kb-930-ms-kit) with the [HP 970 Programmable Wireless Keyboard](https://www.hp.com/us-en/shop/pdp/hp-970-programmable-wireless-keyboard), which the latter is also the same silver as the 930 mouse.
* Other than color (the former is black and the latter is silver), both use the same wireless mouse chassis.

If you choose to use the physical wireless USB transreceiver "dongle", then
remember that you should not loose the dongle.  This is because every dongle is
uniquely paired to the original mouse, so you will not be able to buy a
new dongle to replace the lost dongle.  ([Source](https://h30434.www3.hp.com/t5/Desktop-Hardware-and-Upgrade-Questions/Lost-my-USB-receiver-for-my-wireless-HP-keyboard-and-mouse/td-p/8664321))

## Maintainer metadata
* Architectures: `X86_64`, `aarch64`
* [Link](https://github.com/pop-os/mouse-configurator/releases/latest) to latest GH release
* Checksums: SHA256
    * This is for the source code tarball
    * May change to BLAKE2/`b2sums` in the future
* [AUR package](https://aur.archlinux.org/packages/mouse-configurator)

## Future Plan
* Publish a written review of both mice
* Publish a video version
    * (I'll figure out where to host it later)

## Known issues
The application crashes when importing/exporting the config file on Arch Linux.
See: pop-os/mouse-configurator#24.

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
