# Maintainer: Federico Barcelona <fede.barcelona@sysdig.com>
pkgname=falco
pkgver=0.10.0
pkgrel=1
pkgdesc="Falco, a system-level activity monitoring tool"
arch=("x86_64")
url="http://www.sysdig.org"
license=('GPLv2')
depends=("dkms" "linux-headers")
source=("http://download.draios.com/stable/deb/stable-amd64/$pkgname-$pkgver-x86_64.deb")
md5sums=('281a7d92620a2536ec69b985f717970c')

package() {
	tar xf $srcdir/data.tar.gz -C $pkgdir
}
