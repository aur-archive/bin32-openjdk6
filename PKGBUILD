# Maintainer: c0nd0r <gcesarmza@gmail.com>
pkgname=bin32-openjdk6
pkgver=6.b27_1.12.3
pkgrel=1
pkgdesc="32-bit Free Java environment based on OpenJDK 6.0 with IcedTea6 replacing binary plugs for Arch x86_64"
arch=('x86_64')
license=('custom')
url="http://www.java.net"
depends=('lib32-gcc-libs' 'lib32-libxtst' 'lib32-libxt' 'lib32-nss' 'lib32-libjpeg-turbo' 'lib32-libpng' 'lib32-libxrender' 'ca-certificates-java')
source=(http://mirrors.kernel.org/archlinux/extra/os/i686/${pkgname:6}-$pkgver-$pkgrel-i686.pkg.tar.xz)

md5sums=('f15903d028edc1e665c493db95dca22f')

build() {
  cd ${startdir}/src
  mv usr $pkgdir
  cd $pkgdir/usr
  mv lib lib32
  rm -rf bin
  rm -rf share
}

