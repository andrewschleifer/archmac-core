
pkgname=filesystem
pkgver=2
pkgrel=1
pkgdesc='Base filesystem'
arch=('any')
license=('GPL')
url='http://www.archmac.org'
groups=('base')
source=(profile)
md5sums=('4aaa9ca6b1d0d88e704dd46c1fcea6f8')

package() {
    cd $srcdir

    for dir in bin etc frameworks include lib share var; do
        install -d -m755 $pkgdir/Library/ArchMac/$dir
    done

    install -m644 $srcdir/profile \
        $pkgdir/Library/ArchMac/etc/profile
}
