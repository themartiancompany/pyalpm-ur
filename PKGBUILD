# Maintainer : Rémy Oudompheng <remy@archlinux.org>

pkgname=pyalpm
pkgver=0.8.3
pkgrel=1
pkgdesc="Libalpm bindings for Python 3"
arch=('x86_64')
url="https://git.archlinux.org/pyalpm.git/"
license=('GPL')
makedepends=('git')
depends=('python>=3.6' 'pacman>=5.0')
source=("git+https://git.archlinux.org/pyalpm.git#commit=284d480cd50a0d90dbdd00085efaf0ff9a63913c")
validpgpkeys=('E499C79F53C96A54E572FEE1C06086337C50773E')
sha1sums=('SKIP')

build() {
  cd ${srcdir}/${pkgname}
  python setup.py build
}

package() {
  cd ${srcdir}/${pkgname}
  python setup.py install --root=${pkgdir}
}
