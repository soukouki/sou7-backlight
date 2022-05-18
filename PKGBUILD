# Minatainer: sou7 https://twitter.com/sou7___

pkgname=sou7-backlight
pkgver=0.0.4
pkgrel=0
pkgdesc='A backlight controller'
arch=('any')
url='https://github.com/soukouki/sou7-backlight'
license=('MIT')
depends=('xorg-xbacklight' 'bc')
makedepends=('git')
sha256sums=('SKIP')

pkgver() {
    cd "${srcdir}/"
    git describe --tags | sed 's/^v//;s/-/+/g'
}

package() {
    mkdir "${pkgdir}/usr"
    mkdir "${pkgdir}/usr/bin"
    cp -r "${srcdir}/${pkgdir}/bin/sou7-backlight" "${pkgdir}/usr/bin"
}
