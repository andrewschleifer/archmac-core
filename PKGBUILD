
pkgname=filesystem
pkgver=0.2
pkgrel=3
pkgdesc='Base filesystem'
arch=('any')
license=('GPL')
url='http://www.archmac.org'
groups=('base')
source=(env.sh)
md5sums=('2940f91c69b1bf33ffe3b1115db5be20')

package() {
	cd $srcdir

	for dir in bin etc include lib share var; do
		install -d -m755 $pkgdir/Library/ArchMac/$dir
	done

	mkdir -p $pkgdir/Library/ArchMac/etc/archmac
	install -m644 $srcdir/env.sh \
        $pkgdir/Library/ArchMac/etc/archmac/
}
