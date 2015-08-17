# Contributor: Ryan Coyner <rcoyner@gmail.com>
# Contributor: Laszlo Papp <dj szapi at archlinux us>
# Maintainer: Benjamin A. Shelton <zancarius -at- gmail.com>

# Source: https://github.com/zancarius/archlinux-pkgbuilds

pkgname=python2-openid
pkgver=2.2.5
pkgrel=3
pkgdesc="OpenID library for Python"
arch=(any)
url="http://pypi.python.org/pypi/python-openid/2.2.5"
license=(Apache)
depends=(python2)
makedepends=(python2-distribute)
conflicts=(python-openid)
source=("http://pypi.python.org/packages/source/p/python-openid/python-openid-${pkgver}.tar.gz")
md5sums=(393f48b162ec29c3de9e2973548ea50d)

package () {

    cd "${srcdir}/python-openid-${pkgver}"
    python2 setup.py install --root="${pkgdir}/" --optimize=1
    install -Dm0664 "${srcdir}/python-openid-${pkgver}/LICENSE" "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"

}
