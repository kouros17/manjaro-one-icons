# Creator: Erik Wallström <erik.wallstrom@live.com>
# Maintainer: Fabian Bornschein <plusfabi@gmail.com>

pkgname=pop-icon-theme
pkgver="0.$(date +%Y%m%d)"
pkgrel=1
pkgdesc="A free and open source SVG icon theme for Linux, based on Paper Icon Set and Papirus."
arch=("any")
url="https://github.com/system76/pop-icon-theme"
license=('GPL3')
makedepends=("git")

provides=("${pkgname}")
conflicts=("${pkgname}" "${pkgname}-git")
source=("git+https://github.com/system76/pop-icon-theme.git")
sha512sums=("SKIP")

package() {
  	cd "${pkgname}"
	make DESTDIR="${pkgdir}" install
	make DESTDIR="${pkgdir}" post-install
}

pkgver() {
    printf "0.$(date +%Y%m%d)"
}
