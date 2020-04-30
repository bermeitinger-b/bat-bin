# Maintainer: Bernhard Bermeitinger <bernhard.bermeitinger@gmail.com>

pkgname=bat-cat-bin
pkgver=0.15.0
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
sha256sums=('7b9ee04507c356c336ab4b5af088956255583d612cd5a6b87d4c7bec8fa1dc65')

package() {
  # extract package data
  tar xf data.tar.xz -C "${pkgdir}"

  install -dDm755 "${pkgdir}"/usr/{bin,share}
}
