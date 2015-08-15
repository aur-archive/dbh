# Contributor: aurelien <aurelien@archlinux.org>
pkgname=dbh
pkgver=1.0.24
pkgrel=3
pkgdesc="A library to create Disk Based Hashtables on POSIX systems"
arch=('i686' 'x86_64')
url="http://dbh.sourceforge.net/"
license=('LGPL')
depends=('glibc')
options=('!libtool')
source=(http://downloads.sourceforge.net/sourceforge/$pkgname/$pkgname-$pkgver.tar.gz)
md5sums=('42e122a321089f2429986d0d161ed92a')

build() {
  cd $srcdir/$pkgname-$pkgver
  ./configure --prefix=/usr || return 1
  make || return 1
  make DESTDIR=$pkgdir install || return 1
}
