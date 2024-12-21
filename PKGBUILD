pkgname=dpw
pkgver=1.0.0
pkgrel=1
pkgdesc='Declarative Pacman Wrapper'
arch=(any)
optdepends=('paru: recommended pacman helper')
license=(GPL-3.0-or-later)
source=(dpw)
sha256sums=('9095db5a75e37db6b95dc84cf5e3ddd1459a8636d060d2285b2c04eda7c05fdd')

package() {
	mkdir -p "${pkgdir}/usr/bin"
	cp "${srcdir}/dpw" "${pkgdir}/usr/bin/dpw"
	chmod +x "${pkgdir}/usr/bin/dpw"
}
