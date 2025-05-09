# `ente-cli-bin`

The [CLI](https://github.com/ente-io/ente/tree/main/cli#readme) for Ente allows
users to use CLI commands to manage Ente account backups, for both
[Ente Photos](https://ente.io) and [Ente Auth](https://ente.io/auth), and can
work with [ExifTool](https://en.wikipedia.org/wiki/ExifTool).  The CLI tool was
[announced](https://ente.io/blog/ente-cli/) in November 2023 and is written in
[Go](https://en.wikipedia.org/wiki/Go_(programming_language)).

## Maintainer metadata
* Architecture: `x86_64`, `aarch64`
   * I need to double check `aarch64`, as I'm not as familiar with ARM comparability for Arch Linux
* Use SHA256 checksums for integrity checks
    * Provided by GH releases
* Currently no methods to check authenticity (with GPG)
* [AUR page](https://aur.archlinux.org/packages/ente-cli-bin)
* [Link](https://github.com/ente-io/ente/releases?q=cli&expanded=true) to latest GH release in monorepo
    * Search for `cli` in releases to narrow down results

## Maintenance scope

I will maintain the Ente CLI on the AUR as long as the Ente CLI can't be
installed natively through Arch Linux's `pacman`.

Perhaps I ought to install the Ente CLI package through Go's CLI (like with the
`meme` [tool](https://github.com/nomad-software/meme)), but I think I'll let
this working rule-of-thumb slide, since I currently don't regularly use enough
Go packages to manage through Go's package manager (as I do with Rust crates).
