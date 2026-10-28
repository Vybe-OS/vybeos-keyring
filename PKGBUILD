pkgname=vybeos-keyring
pkgver=1.0
pkgrel=1
pkgdesc='VybeOS PGP keyring'
arch=('any')
url='https://vybeos.dev'
license=('GPL-3.0-or-later')
install=$pkgname.install
source=('vybeos.gpg')
sha256sums=('14e3d2edd9eb8cfa81a7a8beda5b4483499634c5fcba25d34a5f9bb20d6b157a')

package() {
    install -d "${pkgdir}/usr/share/pacman/keyrings"
    
    install -m644 "${srcdir}/vybeos.gpg" "${pkgdir}/usr/share/pacman/keyrings/vybeos.gpg"
}
