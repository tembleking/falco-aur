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
source=("http://download.draios.com/stable/deb/stable-amd64/$pkgname-$pkgver-x86_64.deb"
        "falco.service")
md5sums=('be87172a87bfb2fe55e5d0658499d6b0'
         '7b813b38451df571352ea21d419a15fb')

package() {
    tar xf $srcdir/data.tar.gz -C $pkgdir
    mkdir -p "$pkgdir/usr/lib/systemd/system"
    install -m 0644 falco.service "$pkgdir/usr/lib/systemd/system/falco.service"
}
