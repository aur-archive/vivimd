pkgname=vivimd
pkgver=0.0.4
pkgrel=1
pkgdesc="A wrapper for markdown that attaches vivid styles."
url="https://github.com/peterfyj/vivimd"
arch=("any")
license=("unknown")
depends=("bash" "markdown")
makedepends=("git")
source=("git://github.com/peterfyj/vivimd")
md5sums=("SKIP")
conflicts=()
replaces=()
backup=()

prepare() {
  cd "$srcdir/$pkgname"
  git checkout $pkgver
}

package() {
  cd "$srcdir/$pkgname"
  make install prefix="$pkgdir/usr"
}
