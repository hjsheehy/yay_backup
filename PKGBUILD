# Maintainer: Henry J Sheehy <hjsheehy@gmail.com>
pkgname='yay_backup'
pkgver=1
pkgrel=1
epoch=
pkgdesc="A simple backup tool for yay"
arch=(x86_64)
url="https://github.com/hjsheehy/yay_backup"
license=('GNU')
groups=()
depends=('yay')
makedepends=('git')
source=('https://github.com/hjsheehy/yay_backup.git')
md5sums=('SKIP')

build() {
    echo "$PWD"
	mkdir -p "$pkgname"
	cd "$pkgname"
    echo "$PWD"
	make
}
    # mkdir -p "$pkgdir/usr/bin/$pkgname" "$pkgdir/usr/bin/$pkgname" "$pkgdir/usr/share/doc/$pkgname" "$pkgdir/usr/share/doc/$pkgname"
	# install -dm755 $pkgdir/yay_snapshot "$pkgdir/usr/bin/$pkgname"
	# install -dm755 $pkgdir/yay_restore "$pkgdir/usr/bin/$pkgname"
	# install -dm644 $pkgdir/readme.md "$pkgdir/usr/share/doc/$pkgname"
	# install -dm644 $pkgdir/license "$pkgdir/usr/share/doc/$pkgname"

package() {
    echo "$PWD"
	install -Dm755 ./yay_snapshot "$pkgdir/usr/bin/$pkgname"
	install -Dm755 ./yay_restore "$pkgdir/usr/bin/$pkgname"
	install -Dm644 ./README.md "$pkgdir/usr/share/doc/$pkgname"
	install -Dm644 ./LICENSE "$pkgdir/usr/share/doc/$pkgname"
}
