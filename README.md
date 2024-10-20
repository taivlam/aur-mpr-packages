# My AUR and MPR packages
My [`PKGBUILD`](https://wiki.archlinux.org/title/PKGBUILD) shell scripts for
the [AUR](https://en.wikipedia.org/wiki/Arch_Linux#Arch_User_Repository_(AUR))
and [MPR](https://mpr.makedeb.org/) packages that I maintain

## Repology list (base package names; will use widgets later)
### AUR
* [`meme-cli`](https://repology.org/project/meme-cli/versions)
* [`mudita-center-appimage`](https://repology.org/project/mudita-center/versions)
* [`mouse-configurator`](https://repology.org/project/mouse-configurator/versions)
### MPR
* [`bitwarden-bin`](https://repology.org/project/bitwarden/versions)
* [`electronmail-bin`](https://repology.org/project/electronmail/versions)
* [`ente-auth-bin`](https://repology.org/project/ente-auth/versions)
* [`ente-desktop-bin`](https://repology.org/project/ente-desktop/versions)
* [`ferdium-bin`](https://repology.org/project/ferdium/versions)
* [`freetube-bin`](https://repology.org/project/freetube/versions)
* [`gossip-bin`](https://repology.org/project/gossip-nostr/versions)
* [`organicmaps`](https://repology.org/project/organicmaps/versions) (needs fixing)
* [`playdate-mirror`](https://repology.org/project/playdate-mirror/versions)
* [`proton-mail-bin`](https://repology.org/project/proton-mail/versions)
* [`standard-notes-bin`](https://repology.org/project/standard-notes/versions)
#### Planned
* [`glow`](https://repology.org/project/glow/versions) (uncertain)
    * Also `glow-bin` (uncertain)
* [`jitsi-meet-electron-bin`](https://repology.org/project/jitsi-meet-electron/versions) (soon)
* [`localsend-bin`](https://repology.org/project/localsend/versions) (soon)
* [`playdate-sdk`](https://repology.org/project/playdate-sdk/versions) (TBD)
* [`ricochet-refresh-bin`](https://repology.org/project/ricochet-refresh/versions) (soon)
* [`vnote`](https://repology.org/project/vnote/versions) (WIP)
    * Also `vnote-bin` (WIP)

## Packaging checklist
### Creating/Adopting new package
* Make sure SSH connection is working, as detailed on the "Uploading Packages" [page](https://docs.makedeb.org/using-the-mpr/uploading-packages/)
* Initialize package (implicitly creates repo, if it does not exist yet) with:
  ```
  $ git clone "ssh://mpr@mpr.makedeb.org/<pkg-name-here>.git"
  ```
* Declare Maintainer
    * Denote past Maintainers as Contributors (if needed)
* Change your displayed User Name and E-mail Address for Git repo!
  ```
  $ git config user.name "First-name Last-name"
  $ git config user.email "email@address.here"
  ```
    * Otherwise, you cannot do this [later](https://wiki.archlinux.org/title/AUR_submission_guidelines#Publishing_new_package_content)!
* Confirm e-mail changes the following:
  ```
  $ git config --list  # to see everything (both global first, then local at the end of stdout)
  $ git config user.email  # to see the locally set e-mail address
  ```

### Updating package
* Change:
    * `pkgver`
    * `pkgrel` (if needed)
    * Checksums
        * Most common & cryptographically sound checksums (as of Feb 2024)
            * SHA256
            * SHA512
                * For SHA512 checksums represented by base 64 in YAML files, use the following command to convert from hexadecimal into base 64:
                  ```
                  $ sha512sum <binary-name>.deb | cut -f1 -d\  | xxd -r -p | base64 -w0
                  ```
            * [BLAKE2](https://en.wikipedia.org/wiki/BLAKE_(hash_function)#Users_of_BLAKE2) (i.e., the `b2sum` command in GNU Core Utilities)
        * Download the specified archive from the source (e.g. GitHub, GitLab, direct software source page, & so on)
* Update `.SRCINFO` package metadata file with:
  ```
  $ makepkg --printsrcinfo | tee .SRCINFO
  ```
    * This will print `.SRCINFO` (the `PKGBUILD` metadata that is used for the web page) into stdout (which helps to tell if the output `source` links work correctly.
* Lastly, add the files, make a commit, and push the changes:
  ```
  $ git add .
  $ git commit -m "Add message here"
  $ git commit --amend    # Write a longer message here, if needed
  $ git push
  ```
### Sources
* [AUR](https://wiki.archlinux.org/title/Arch_User_Repository) on the ArchWiki
    * [AUR Submission Guidelines](https://wiki.archlinux.org/title/AUR_submission_guidelines) on the ArchWiki
* [`.SRCINFO`](https://wiki.archlinux.org/title/.SRCINFO) on the ArchWiki
* `makedeb` documentation [page](https://docs.makedeb.org/using-the-mpr/uploading-packages/) on uploading packages to the MPR

## License
The [license](LICENSE) for the `PKGBUILD` scripts I author are under the GNU
General Public License Version 3
([GNU GPLv3](https://en.wikipedia.org/wiki/GNU_General_Public_License#Version_3)).
