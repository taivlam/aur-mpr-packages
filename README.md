# My AUR and MPR packages
My [`PKGBUILD`](https://wiki.archlinux.org/title/PKGBUILD) shell scripts for
the [AUR](https://en.wikipedia.org/wiki/Arch_Linux#Arch_User_Repository_(AUR))
and [MPR](https://mpr.makedeb.org/) packages that I maintain

## Repology list (base package names; will use widgets later)
### AUR
* [`mudita-center-appimage`](https://repology.org/project/mudita-center/versions)
* [`mouse-configurator`](https://repology.org/project/mouse-configurator/versions)
### MPR
* [`bitwarden-bin`](https://repology.org/project/bitwarden/versions)
* [`electronmail-bin`](https://repology.org/project/electronmail/versions)
* [`ente-auth-bin`](https://repology.org/project/ente-auth/versions)
* [`ente-desktop-bin`](https://repology.org/project/ente-desktop/versions) (soon)
* [`ferdium-bin`](https://repology.org/project/ferdium/versions)
* [`freetube-bin`](https://repology.org/project/freetube/versions)
* [`organicmaps`](https://repology.org/project/organicmaps/versions) (needs fixing)
* [`proton-mail-bin`](https://repology.org/project/proton-mail/versions) (soon)
#### Planned
* [`glow`](https://repology.org/project/glow/versions) (uncertain)
    * Also `glow-bin` (uncertain)
* [`playdate-mirror`](https://repology.org/project/playdate-mirror/versions) (TBD)
* [`playdate-sdk`](https://repology.org/project/playdate-sdk/versions) (TBD)
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
            * [BLAKE2](https://en.wikipedia.org/wiki/BLAKE_(hash_function)#Users_of_BLAKE2) (i.e., the `b2sum` command in GNU Core Utilities)
        * Download the specified archive from the source (e.g. GitHub, GitLab, direct software source page, & so on)
* Update `.SRCINFO` package metadata file with:
  ```
  $ makepkg --printsrcinfo > .SRCINFO
  ```
* Lastly, add the files, make a commit, and push the changes:
  ```
  $ git add .
  $ git commit -m "Add message here"
  $ git commit --amend    # Write a longer message here, if needed
  $ git push
  ```
### Sources from the ArchWiki
* [AUR](https://wiki.archlinux.org/title/Arch_User_Repository)
    * [AUR Submission Guidelines](https://wiki.archlinux.org/title/AUR_submission_guidelines)
* [`.SRCINFO`](https://wiki.archlinux.org/title/.SRCINFO)

## License
The [license](LICENSE) for the `PKGBUILD` scripts I author are under the GNU
General Public License Version 3
([GNU GPLv3](https://en.wikipedia.org/wiki/GNU_General_Public_License#Version_3)).
