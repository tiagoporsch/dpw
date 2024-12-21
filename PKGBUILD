pkgname=dpw
pkgver=1.1.0
pkgrel=1
pkgdesc='Declarative Pacman Wrapper'
arch=(any)
optdepends=('paru: recommended pacman helper')
license=(GPL-3.0-or-later)
source=(dpw dpw.fish)
sha256sums=('3195adf1f9af8bd55546191008aa1b4af9049feb4e28ec9837673be89b115504' 'c2b828519653d3f2280d4904d7ad8924d2671986c9ad33af17ff60fba83522a1')

package() {
	mkdir -p "${pkgdir}/usr/bin"
	cp "${srcdir}/dpw" "${pkgdir}/usr/bin/dpw"
	chmod +x "${pkgdir}/usr/bin/dpw"

	# Add fish completions if fish shell is installed
	if [ -x "$(command -v fish)" ]; then
		if [ -d "/usr/share/fish/vendor_completions.d" ]; then	
			mkdir -p "/usr/share/fish/vendor_completions.d"
		fi

		sudo cp "${srcdir}/dpw.fish" "/usr/share/fish/vendor_completions.d/dpw.fish"
	fi
}
