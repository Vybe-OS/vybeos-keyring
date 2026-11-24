pkgname=vybeos-keyring
pkgver=2.0
pkgrel=1
pkgdesc='VybeOS PGP keyring'
arch=('any')
url='https://vybeos.dev'
license=('GPL-3.0-or-later')
install=$pkgname.install
source=(
    'vybeos.gpg'
    'vybeos-trusted'
    'vybeos-revoked'
    'vybeos-mirrorlist'
)
sha256sums=('14e3d2edd9eb8cfa81a7a8beda5b4483499634c5fcba25d34a5f9bb20d6b157a'
            '8836b7cd106771dd026c8285c49eafc8d5b053d212fc4409eaaa484400cc9f38'
            'e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855'
            '0e1ca687f3481a5727577985eac436ff40c1dd126dcef227153fa68403ac5257')

package() {
    install -d "${pkgdir}/usr/share/pacman/keyrings"
    
    install -m644 "${srcdir}/vybeos.gpg" "${pkgdir}/usr/share/pacman/keyrings/vybeos.gpg"
    install -m644 "${srcdir}/vybeos-trusted" "${pkgdir}/usr/share/pacman/keyrings/vybeos-trusted"
    install -m644 "${srcdir}/vybeos-revoked" "${pkgdir}/usr/share/pacman/keyrings/vybeos-revoked"
    install -Dm644 "${srcdir}/vybeos-mirrorlist" "${pkgdir}/etc/pacman.d/vybeos-mirrorlist"
}
