# Maintainer David Freitag <dvdfreitag@gmail.com>

pkgname=xfce4-systemload-plugin
pkgver=1.2.4dovid
pkgrel=1
pkgdesc='A system load plugin for the Xfce4 panel'
arch=('i686' 'x86_64')
license=('GPL')
url='https://github.com/dvdfreitag/xfce4-systemload-plugin'
groups=('xfce4-goodies')
depends=('xfce4-panel' 'upower')
conflicts=('xfce4-systemload-plugin')
provides=('xfce4-systemload-plugin')
makedepends=('xfce4-dev-tools' 'intltool' 'git')
options=('!libtool')
install=xfce4-systemload-plugin.install
source=('https://github.com/dvdfreitag/xfce4-systemload-plugin/archive/1.2.4dovid.tar.gz')
sha256sums=('0a860eb28e4f8ffe26e5676d9bc2c83e0a0ff04ad53990ebedce5720a7237cfc')

build() {
	cd "$pkgname-$pkgver"/

	./autogen.sh --prefix=/usr \
		--sysconfdir=/etc \
		--libexecdir=/usr/lib \
		--localstatedir=/var \
		--disable-static \
		--enable-maintainer-mode \
		--disable-debug

	make
}

package() {
	cd "$pkgname-$pkgver"
	make DESTDIR="${pkgdir}" install
}
