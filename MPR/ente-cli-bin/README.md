# `ente-cli-bin`

The [CLI](https://github.com/ente-io/ente/tree/main/cli#readme) for Ente allows
users to use CLI commands to manage Ente account backups, for both
[Ente Photos](https://ente.io) and [Ente Auth](https://ente.io/auth), and can
work with [ExifTool](https://en.wikipedia.org/wiki/ExifTool).  The CLI tool was
[announced](https://ente.io/blog/ente-cli/) in November 2023 and is written in
[Go](https://en.wikipedia.org/wiki/Go_(programming_language)).

## Maintainer metadata
* Architecture: `amd64`
    * Most likely `arm64` - but I need to double check, as I'm not as familiar with ARM comparability for Arch Linux
* Use SHA256 checksums for integrity checks
    * Provided by GH releases
* Currently no methods to check authenticity (with GPG)
* [MPR page](https://mpr.makedeb.org/pkgbase/ente-cli-bin)

## Maintenance scope

I will maintain the Ente CLI on the MPR as long as the Ente CLI can't be
installed natively through Debian's/Ubuntu's APT.

Perhaps I ought to install the Ente CLI package through Go's CLI (like with the
`meme` [tool](https://github.com/nomad-software/meme)), but I think I'll let
this working rule-of-thumb slide, since I currently don't regularly use enough
Go packages to manage through Go's package manager (as I do with Rust crates).
I also don't have experience installing Go packages via the CLI on APT-based
Linux distros.
