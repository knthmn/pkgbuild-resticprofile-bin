# Maintainer: Kent Hou Man <knthmn0 at gmail dot com>
pkgname=resticprofile-bin
pkgver=0.28.0
pkgrel=1
pkgdesc="Configuration profiles for restic backup. Pre-compiled"
arch=('x86_64' 'aarch64' 'armv6h' 'armv7h')
url="https://github.com/creativeprojects/resticprofile"
license=('GPL3')
depends=(
  'restic'
)
provides=('resticprofile')
conflicts=('resticprofile')

source_x86_64=("https://github.com/creativeprojects/resticprofile/releases/download/v${pkgver}/resticprofile_${pkgver}_linux_amd64.tar.gz")
source_aarch64=("https://github.com/creativeprojects/resticprofile/releases/download/v${pkgver}/resticprofile_${pkgver}_linux_arm64.tar.gz")
source_armv6h=("https://github.com/creativeprojects/resticprofile/releases/download/v${pkgver}/resticprofile_${pkgver}_linux_armv6.tar.gz")
source_armv7h=("https://github.com/creativeprojects/resticprofile/releases/download/v${pkgver}/resticprofile_${pkgver}_linux_armv7.tar.gz")

sha256sums_x86_64=('8a8b8c611ea86beb9eb095417e851c88e3f1f9e2fda894ea9b2664a94368716a')
sha256sums_aarch64=('3cfab1f2e2c744a750777d61747de67d96e0b9419783d6f0ca708ddfc97e5817')
sha256sums_armv6h=('968c89c09075f23ec2e97240c723ece560e504c50836b0694da879833ed9b46a')
sha256sums_armv7h=('e252989194b870d79e1a267f75dee5b9707782d8012abb9b40747e0bb6c2140a')

package() {
  install -Dm755 "${srcdir}/resticprofile" "${pkgdir}/usr/bin/resticprofile" 
  install -Dm644 "${srcdir}/LICENSE" "${pkgdir}/usr/share/licenses/resticprofile/LICENSE"
  install -Dm644 "${srcdir}/README.md" "${pkgdir}/usr/share/doc/resticprofile/README.md"
}
