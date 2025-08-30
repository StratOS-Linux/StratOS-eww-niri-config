# Maintainer: @zstg <o0vckutt@duck.com>
pkgname=stratos-eww-config
pkgver=1.0
pkgrel=3
pkgdesc="Eww configuration for StratOS"
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
	cp -r $startdir/usr $srcdir/
}

source=()
install=stratos-eww-config.install

package() {
    install -d $pkgdir/etc/skel/.config/
    install -d $pkgdir/usr/local/bin/
    cp -ra $srcdir/.config/eww/ $pkgdir/etc/skel/.config/
    cp -ra $srcdir/usr/local/bin/eww-toggle $pkgdir/usr/local/bin/
}
