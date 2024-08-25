# `ente-desktop-bin`

## Maintainer metadata
* Architectures: `amd64`, `arm64`
* SHA512 checksums in base 64 form in published auto-generated YAML files
    * See ente-io/ente#2805 for discussion
    * Use the following one-line command on the binary executable:
      ```
      $ sha512 <latest-binary-name>.deb | cut -f1 -d\  | xxd -r -p | base64 -w0
      ```

## About
[Ente](https://ente.io/) first started out making a client for end-to-end
encrypted photo storage.  Currently, code for both client and server code is
open-source.  This is its desktop client on APT-based Linux distros.  The
creators of Ente Photos also created [Ente Auth](https://ente.io/auth/).

## Scope
I will maintain this package until Ente officially support an automatically
updating method (such as a third-party APT repository) for Debian/Ubuntu.

