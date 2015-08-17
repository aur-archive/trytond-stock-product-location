# Maintainer: Robin Baumgartner <robin@baumgartners.ch>
pkgname=trytond-stock-product-location
_pkgname=trytond_stock_product_location
pkgver=3.4.1
_pkgdir=3.4
pkgrel=1
pkgdesc="The stock_product_location module of the Tryton application platform"
arch=('any')
url='http://www.tryton.org/'
license=('GPL3')
groups=('trytond-modules')
depends=('trytond>=3.4' 'trytond-product>=3.4' 'trytond-stock>=3.4')
makedepends=('python2-distribute')
source=("http://downloads.tryton.org/$_pkgdir/$_pkgname-$pkgver.tar.gz")
md5sums=("b97a17c9cb043bbf2da2c144ba1e138c")

build() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py build
}

package() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py install --root=$pkgdir
}