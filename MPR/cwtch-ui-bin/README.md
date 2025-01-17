# `cwtch-ui-bin`

## Maintainer metadata
* Platform: only `amd64` (presumably)
* [Link](https://git.openprivacy.ca/cwtch.im/cwtch-ui/releases/latest) to latest release on Gitea
* No integrity checks currently
    * So use BLAKE2 checksums
* Currently no authenticity checks (with GPG tools)
* [Link](https://git.openprivacy.ca/cwtch.im/cwtch-ui/releases/latest) to latest release on Gitea
* MPR package [page](https://mpr.makedeb.org/packages/cwtch-ui-bin)

### Suggestion for install `tor` dependency

### Suggestion for install `tor` dependency

As one of the runtime dependencies is `tor`, I suggest following the 
[instructions](https://support.torproject.org/apt/) from the Tor Project to add its APT repo to
your system.

## Context and background info

Cwtch is a decentralized and metadata resistant E2EE communication app designed by
[Open Privacy Research Society](https://openprivacy.ca/).  The desktop UI application is what users
will use to communicate over Cwtch.  (On the other hand, the `cwtch` software is the
[software](https://git.openprivacy.ca/cwtch.im/cwtch) for the Cwtch protocol.)  Cwtch also uses
[Tor](https://en.wikipedia.org/wiki/Tor_(network)).

Its source code [repo](https://git.openprivacy.ca/cwtch.im/cwtch-ui) is on Open Privacy's
self-hosted [Gitea](https://en.wikipedia.org/wiki/Gitea) instance.

### Maintenance scope

I will maintain this package as long as there isn't an auto-updating method for DEB archive
binaries.
