
pkgname=archmac
pkgver=2
pkgrel=19
pkgdesc='Base filesystem'
arch=(any)
license=(GPL)
url='http://www.archmac.org'
groups=(base)
source=(profile)
replaces=(filesystem)
conflicts=(filesystem)
md5sums=(3ff089d102da0872f409811dd742cbda)

package() {
    cd $srcdir

    for dir in bin etc frameworks include info lib man share var; do
        install -d -m755 $pkgdir/Library/ArchMac/$dir
    done

    install -m644 $srcdir/profile \
        $pkgdir/Library/ArchMac/etc/profile
}

