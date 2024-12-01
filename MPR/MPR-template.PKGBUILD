# Maintainer: Tai Lam <taivlam-aur-mpr [dot] tinsmith796 [at] silomails [dot] com>

_pkgname="<_pgkname>"
pkgname="<_pgkname>-bin"  # Adjust accordingly, if not precompiled binary
pkgver='0.0.0'
pkgrel='0'
pkgdesc="<Forge repo description>"
arch=('amd64' 'arm64')  # Adjust architecture platforms accordingly
depends=()
license=('<license>')
url="<usually-human-readable-site>"
#_url="<link-to-forge-repo>"  # If not unique, then modify symbolic variables below; set up for GH
source_amd64=("${pkgname}_${pkgver}-${pkgrel}_${arch}.deb"::"${_url}/releases/download/v${pkgver}/${_pkgname}-v${pkgver}-linux-amd64.deb")
source_ard64=("${pkgname}_${pkgver}-${pkgrel}_${arch}.deb"::"${_url}/releases/download/v${pkgver}/${_pkgname}-v${pkgver}-linux-arm64.deb")
sha256sums_amd64=('<checksum-for-amd64>')
sha256sums_arm64=('<checksum-for-arm64>')
noextract=("${pkgname}_${pkgver}-${pkgrel}_${arch}.deb")
provides=("${_pkgname}")
conflicts=("<_pgkname>" "<_pgkname>-deb")

package() {
exec true
}
