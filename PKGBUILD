# Maintainer: Stefan Zipproth <s.zipproth@ditana.org>

pkgname=ditana-testing-mirrorlist
pkgver=1.12
pkgrel=1
pkgdesc="Ditana testing mirrorlist for pacman"
arch=(any)
url="https://ditana.org"
license=('AGPL-3.0-or-later')
conflicts=()
depends=()
makedepends=()
source=("file://${PWD}/ditana-testing-mirrorlist")
sha256sums=('SKIP')

package() {
    install -D -m644 $srcdir/ditana-testing-mirrorlist $pkgdir/etc/pacman.d/ditana-testing-mirrorlist
}
