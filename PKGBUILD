# Maintainer: Bernhard Bermeitinger <bernhard.bermeitinger@gmail.com>

pkgname=bat-cat-bin
pkgver=0.13.0
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
sha256sums=('70aa43695bb0fcf278999838d6b9e37356a170fea1cb866feaa927a1e709f3a0')

package() {
  # extract package data
  tar xf data.tar.xz -C "${pkgdir}"

  install -dDm755 "${pkgdir}"/usr/{bin,share}
}
