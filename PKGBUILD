# Maintainer: Bernhard Bermeitinger <bernhard.bermeitinger@gmail.com>

pkgname=bat-cat-bin
pkgver=0.15.1
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
sha256sums=('fb287c4e14bb945d660d5cb10f3b2e072a65f2b02a73a404939c65fb3e57a931')

package() {
  # extract package data
  tar xf data.tar.xz -C "${pkgdir}"

  install -dDm755 "${pkgdir}"/usr/{bin,share}
}
