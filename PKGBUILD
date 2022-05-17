# Minatainer: sou7 https://twitter.com/sou7___

pkgname=sou7-backlight
pkgver=0.0.0
pkgrel=1
pkgdesc='A backlight controler'
arch=('any')
url='https://github.com/soukouki/sou7-backlight'
license=('MIT')
depends=('xorg-xbacklight' 'bc')
makedepends=('git')
source=("git+${url}.git#tag=v${pkgver}")
sha256sums=('SKIP')

pkgver() {
    cd "${srcdir}/${pkgname}"
    git describe --tags | sed 's/^v//;s/-/+/g'
}

package() {
    mkdir "${pkgdir}/usr"
    mkdir "${pkgdir}/usr/bin"
    cp -r "${srcdir}/${pkgname}/sou7-backlight" "${pkgdir}/usr/bin"
}
