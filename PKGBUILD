# Maintainer: Michael P <ptchinster@archlinux.us>
pkgname=hamster
pkgver=2.0.0
pkgrel=10
pkgdesc="Tool for HTTP session sidejacking."
arch=('i686' 'x86_64')
url="http://hamster.erratasec.com/"
license=('GPL')
groups=()
depends=('libpcap')
makedepends=(unzip)
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=(http://www.clshack.it/nopaste/hamster-2.0.0.zip)
noextract=()
md5sums=('0f302f3890225d9698bd9b964888d577')

build() {
	mkdir -p ${pkgdir}/opt/hamster

	cd ${srcdir}/hamster/build/gcc4
	make
	cp ../../bin/* ${pkgdir}/opt/hamster

	cd ${srcdir}/ferret/build/gcc4
	make
	cp ../../bin/* ${pkgdir}/opt/hamster
}

