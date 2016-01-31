pkgname=wps-office-i18-es-es
pkgver=10.1.0.5460_a20p1
_pkgver=10.1.0.5460
_pkgrel=~a20p1
pkgrel=1
pkgdesc="i18n es-es files for wps-office"
arch=('x86_64')
license=("custom")
url="http://wps-community.org/"
depends=('wps-office')
options=('!emptydirs')
source=("http://kdl.cc.ksosoft.com/wps-community/download/mui/${_pkgver}/mui_es_es.7z"
        "http://wps-community.org/download/dicts/es_ES.zip")
sha512sums=('1bfc1cf61cae83d2b0c3c3babdf684ca265ca0dedcf02896cb104adf281d359786e677c478039f6790f7a1a6329fd4205ebf4b6b7ace9d5cb4a999dc23257aea'
            '0c9cae3f4bae8c61eb6c6c060f12271d20f383b453387c1e3c829bb79fd309b83ac3d655a10ad57f88d8637f18903361bdb4b04660a563ee84b56b6f4f1cef01')

package() {
  cd $srcdir

  install -d "$pkgdir/usr/lib"
  cp -r office6 "$pkgdir/usr/lib"
  cp -r es_ES "$pkgdir/usr/lib/office6/dicts"
}
