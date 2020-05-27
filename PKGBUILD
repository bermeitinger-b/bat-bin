# Maintainer: Bernhard Bermeitinger <bernhard.bermeitinger@gmail.com>

pkgname=bat-cat-bin
pkgver=0.15.4
pkgrel=1
pkgdesc='A cat(1) clone with wings.'
arch=('x86_64')
url='https://github.com/sharkdp/bat'
license=('Apache')
depends=('gcc-libs' 'zlib')
optdepends=()
provides=('bat-cat')
conflicts=('bat-cat-git')
options=('!strip')
source=("https://github.com/sharkdp/bat/releases/download/v${pkgver}/bat_${pkgver}_amd64.deb")
sha256sums=('66b5fa31e4946da9331824fba4b6a7076565fe83866f14562450a010a5112857')

package() {
  # extract package data
  tar xf data.tar.xz -C "${pkgdir}"

  install -dDm755 "${pkgdir}"/usr/{bin,share}
}
