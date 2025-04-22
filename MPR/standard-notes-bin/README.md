# `standard-notes-bin`

## Maintainer metadata
* Architecture: `amd64`, `arm64`
* Look for the latest desktop release on [GH releases](https://github.com/standardnotes/app/releases)
    * This is a monorepo for the other client applications, such as the mobile app and the clipper browser extension
    * So, [search](https://github.com/standardnotes/app/releases?q=desktop&expanded=true) for only desktop releases with "`desktop`"
* YAML files provide SHA512 checksums in base 64 form
    * SHA256 checksums also offered, but not preferred
* [MPR page](https://mpr.makedeb.org/packages/standard-notes-bin)

## Motivation and scope
I decided to package this, as `.deb` archives/binary executables for Standard
Notes were produced via GitHub releases, but not through the website itself.
(Only the AppImage is explicitly mentioned on Standard Note's website.)

I wanted to use a trusted cloud-based, E2EE, and cross-platform notes
application, as I keep loosing notes on [gedit](https://en.wikipedia.org/wiki/Gedit)
whenever my laptop looses battery power.

I will maintain this package as long as Standard Notes's official support and
site doesn't provide an auto-updating way to install Standard Notes on
Debian/Ubuntu through `.deb` archives.

## Background
[Standard Notes](https://standardnotes.com/) is an E2EE cloud-based note
application.  The business behind Standard Notes was acquired by Proton Tech in
April 2024 (c.f. the respective statements from
[Proton](https://proton.me/blog/proton-standard-notes-join-forces) and
[Standard Notes](https://standardnotes.com/blog/joining-forces-with-proton)).

### Speculation
This is probably a long-term strategy move that Proton Tech is making so that a
Google Docs-like collaborative platform can be made to be increasingly
comparable with the "standard" set of the Google Suite (so, GMail, Google Docs,
and Google Drive would be my top three picks). 

