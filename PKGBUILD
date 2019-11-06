# Maintainer: Bernhard Bermeitinger <bernhard.bermeitinger@gmail.com>

pkgname=bat-cat-bin
pkgver=0.12.1
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
sha256sums=('c02ca23add052009cde64746ff86e6da5765a89fd7494d380800250310180b23')

package() {
  # extract package data
  tar xf data.tar.xz -C "${pkgdir}"

  install -dDm755 "${pkgdir}"/usr/{bin,share}
}
