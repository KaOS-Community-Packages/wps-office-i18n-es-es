pkgname=wps-office-i18-es-es
pkgver=10.1.0.5503_a20p2
_pkgver=10.1.0.5503
_pkgrel=~a20p2
pkgrel=1
pkgdesc="i18n es-es files for wps-office"
arch=('x86_64')
license=("custom")
url="http://wps-community.org/"
depends=('wps-office')
options=('!emptydirs')
source=("http://kdl.cc.ksosoft.com/wps-community/download/mui/${_pkgver}/mui_es_es.7z"
        "http://wps-community.org/download/dicts/es_ES.zip")
sha512sums=('18b623ac38d83afe5c721a8d7a3013ff5876e552a3692a14af14545d61be56764e6b665d51fd4865b64f84e7d45167c289759f3a95cf60b4b00af9c7d22cd735'
            '0c9cae3f4bae8c61eb6c6c060f12271d20f383b453387c1e3c829bb79fd309b83ac3d655a10ad57f88d8637f18903361bdb4b04660a563ee84b56b6f4f1cef01')

package() {
  cd $srcdir

  install -d "$pkgdir/usr/lib"
  cp -r office6 "$pkgdir/usr/lib"
  cp -r es_ES "$pkgdir/usr/lib/office6/dicts"
}
