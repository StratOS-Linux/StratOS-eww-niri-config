# Maintainer: @magitian <magitian@duck.com>
pkgname=stratos-eww-niri-config
pkgver=1.0
pkgrel=1
pkgdesc="Eww configuration for StratOS' Niri spin"
arch=('any')
license=('GPL3')
depends=(
  'eww'
)

optdepends=( 
  'stratos-bin: Additional scripts used in StratOS'
)

prepare() {
	cp -r $startdir/.config/ $srcdir/
}

source=()
install=stratos-eww-config.install

package() {
    install -d $pkgdir/etc/skel/.config/
    cp -ra $srcdir/.config/eww/ $pkgdir/etc/skel/.config/
}
