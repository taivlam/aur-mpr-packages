# `freetube-bin`
## Maintainer metadata
* Architectures: `amd64`, `arm64`
    * Apparently `armv7l` is generated, but MPR doesn't recognize it
* No checksums offered
    * So, use BLAKE2 checksums (`b2sums`)
* [MPR page](https://mpr.makedeb.org/packages/freetube-bin)
* [GH tags](https://github.com/FreeTubeApp/FreeTube/tags)
    * No GH releases, only tags
    * Nominally uses "pre-release" label on GH
        * But treat as stable production release for packaging purposes
    * Officially FreeTube is "beta" software

## Background and context
[FreeTube](https://freetubeapp.io/) is a third-party desktop client for YouTube.

FreeTube is available for Windows, MacOS, and Linux and is based on
[Electron](https://en.wikipedia.org/wiki/Electron_(software_framework)).

I use FreeTube because it avoids YouTube's ads.  Also, even if you use
[uBlock Origin](https://en.wikipedia.org/wiki/UBlock_Origin), YouTube's vanilla
website UI runs sluggishly (for a website in 2020 and onward) and is slowed down
by unnecessary amounts of JavaScript running the recommended video columns and
other needless UI clutter.

## Maintaining this MPR package

I took over maintaining this MPR package because there is no official method yet
from FreeTube to install on Debian-/Ubuntu-based Linux distros via a third-party
[APT](https://en.wikipedia.org/wiki/APT_(software)) repository - see
FreeTubeApp/FreeTube#871 for progress on this.

If that were to ever happen and the project decides to officially move away from
the MPR for Debian-/Ubuntu-based installations, then I would stop maintaining
this package.

## Thanks
Thanks to the prior maintainer, [@hiddeninthesand](https://github.com/hiddeninthesand),
for starting this package.
