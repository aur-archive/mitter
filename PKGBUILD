# Maintainer: Jaroslav Lichtblau <dragonlord@aur.archlinux.org>
# Contributor: Geoffroy Carrier <geoffroy.carrier@koon.fr>

pkgname=mitter
pkgver=0.4.5
pkgrel=3
pkgdesc="A PyGTK/console client for Twitter"
arch=('any')
url="http://code.google.com/p/mitter/"
license=('GPL3')
depends=('python2' 'pygtk')
source=(http://$pkgname.googlecode.com/files/$pkgname-$pkgver.tar.gz)
md5sums=('0432f3d2d00e8d048bf0839e2d857e51')

package() {
  cd ${srcdir}/$pkgname-$pkgver

  python2 setup.py install --root=${pkgdir}
  install -D -m644 ${pkgname}.desktop ${pkgdir}/usr/share/applications/${pkgname}.desktop
}
