# Maintainer: Michał Walczak <michalwalczak at michalwalczak dot eu>

pkgname=stodo
pkgver=1.1.3
pkgrel=1
pkgdesc="A simple CLI todo application"
arch=('any')
url="http://github.com/magikmw/stodo"
license=('GPL3+')
depends=('python' 'sqlite')
source=(http://michalwalczak.eu/stuff/stodo/stodo-$pkgver.tar.gz)
md5sums=('67a52389a16c520c1716bb587cbb20e2')
install="stodo.install"

package() {
  _docs_dir="$pkgdir/usr/share/doc/$pkgname"
  _bin_dir="$pkgdir/usr/bin"
  mkdir -p $_docs_dir
  mkdir -p $_bin_dir

  cd "$srcdir"

  install -D -m 755 stodo "$_bin_dir"
  install -D -m 644 README "$_docs_dir"
  install -D -m 644 LICENSE "$_docs_dir"
}
