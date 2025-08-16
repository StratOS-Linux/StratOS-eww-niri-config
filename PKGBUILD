# Maintainer: @magitian <magitian@duck.com>
pkgname=stratos-eww-config
pkgver=1.0
pkgrel=1
pkgdesc="Eww configuration for StratOS"
arch=('any')
license=('GPL3')
depends=(
)

optdepends=( 
)

prepare() {
	cp -r "$startdir/.config/" "$srcdir/"
}

source=()
install=stratos-eww-config.install

package() {
    install -d "$pkgdir/etc/skel/.config"
    cp -r "$srcdir/.config/eww/" "$pkgdir/etc/skel/.config/"
}