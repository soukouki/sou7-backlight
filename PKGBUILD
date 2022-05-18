# Minatainer: sou7 https://twitter.com/sou7___

pkgname=sou7-backlight
pkgver=0.0.2
pkgrel=1
pkgdesc='A backlight controller'
arch=('any')
url='https://github.com/soukouki/sou7-backlight'
license=('MIT')
depends=('xorg-xbacklight' 'bc')
makedepends=('git')
srcdir="${pkgname}-${pkgver}"
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
