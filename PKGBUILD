# Maintainer: Nathaniel Case <qalthos@gmail.com>
pkgname=pyrasite
pkgver=2.0beta4
pkgrel=1
pkgdesc="Code injection and introspection of running Python processes"
arch=('i686' 'x86_64')
url="http://pyrasite.com"
license=('GPL3')
depends=('python2' 'python2-meliae' 'python2-sphinx' 'python2-psutil' 'libwebkit3' 'graphviz')
source=(http://pypi.python.org/packages/source/p/pyrasite/pyrasite-$pkgver.tar.gz)
md5sums=('218d05f509fee9d9111256f6146be3ae')

build() {
  cd $startdir/src/$pkgname-$pkgver
  python2 ./setup.py install --root=$pkgdir
  sed -i -e 's,^#!/usr/bin.*,#!/usr/bin/env python2,' $pkgdir/usr/bin/*
}

# vim:set ts=2 sw=2 et:
