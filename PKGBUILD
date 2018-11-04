# Maintainer: Federico Barcelona <fede.barcelona@sysdig.com>
pkgname=falco
pkgver=0.12.1
pkgrel=1
pkgdesc="Falco, a system-level activity monitoring tool"
arch=("x86_64")
url="http://www.sysdig.org"
license=('GPL2')
depends=("dkms" "linux-headers")
backup=("etc/falco/falco.yaml" "etc/falco/falco_rules.local.yaml")
source=("http://download.draios.com/stable/deb/stable-amd64/$pkgname-$pkgver-x86_64.deb")
md5sums=('be87172a87bfb2fe55e5d0658499d6b0')

package() {
	tar xf $srcdir/data.tar.gz -C $pkgdir
}
