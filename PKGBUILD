pkgname=vybeos-keyring
pkgver=20261028
pkgrel=1
pkgdesc='VybeOS PGP keyring'
arch=('any')
url='https://vybeos.dev'
license=('GPL-3.0-or-later')
install=$pkgname.install
source=('vybeos.gpg' 'vybeos-trusted' 'vybeos-revoked')
sha256sums=('14e3d2edd9eb8cfa81a7a8beda5b4483499634c5fcba25d34a5f9bb20d6b157a'
            '73cbd1f14f4fc7e3f376f245e8e3fd0a3dcebf02d38824939ecd4a47a4384ec1'
            'e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855')

package() {
    install -Dm644 vybeos.gpg vybeos-trusted vybeos-revoked \
        -t "$pkgdir/usr/share/pacman/keyrings/"
}
