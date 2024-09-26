pkgname=cinnamon-configs
_destname1="/src"
pkgver=1
pkgrel=1
pkgdesc="Desktop Config for Acreetion OS"
arch=('any')
url="https://github.com/cobra3282000"
license=('GPL3')
makedepends=('git')
conflicts=()
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${pkgname}::"git+${url}/${pkgname}")
sha256sums=('SKIP')
package() {
	install -dm755 ${pkgdir}${_destname1}
	cp -r ${srcdir}/${pkgname}${_destname1}/* ${pkgdir}${_destname1}
	rm ${srcdir}/${pkgname}/git_clean.sh
	rm ${srcdir}/${pkgname}/git_push.sh
	rm ${srcdir}/${pkgname}/git_setup.sh
	rm ${srcdir}/${pkgname}/PKGBUILD
}
