# Maintainer: alucryd <alucryd at gmail dot com>
# Maintainer: josephgbr <rafael.f.f1 at gmail dot com>

pkgname=lib32-nvidia-cg-toolkit
pkgver=3.1
pkgrel=3
pkgdesc="NVIDIA Cg libraries"
arch=('x86_64')
url="http://developer.nvidia.com/object/cg_toolkit.html"
license=('custom')
depends=('lib32-mesa' "${pkgname#*-}")
source=("http://developer.download.nvidia.com/cg/Cg_${pkgver}/Cg-${pkgver}_April2012_x86.tgz")
sha256sums=('cef3591e436f528852db0e8c145d3842f920e0c89bcfb219c466797cb7b18879')

package() {
  install -dm 755 "${pkgdir}"/usr/lib32
  install -m 644 "${srcdir}"/usr/lib/* "${pkgdir}"/usr/lib32

# License
  install -dm 755 "${pkgdir}"/usr/share/licenses
  ln -s "${pkgname#*-}" "${pkgdir}"/usr/share/licenses/${pkgname}
}

# vim: ts=2 sw=2 et:
