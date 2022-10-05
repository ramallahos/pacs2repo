# Maintainer: Safwan Nayeem Yousuf <safwannayeemyousuf.com>
pkgname=pacs2repo
pkgver=1
pkgrel=1
pkgdesc="List all provided packages with their respective repositories."
arch=('any')
url="https://github.com/ramallahos/$pkgname"
license=('MIT')
optdepends=('paru')
makedepends=('coreutils')
backup=('etc/pacman.conf')
source=("$pkgname::git+$url.git")
sha256sums=('SKIP')

package() {
    cd "$pkgname"
    install -Dm755 pacs2repo "$pkgdir/usr/bin/pacs2repo"
    install -Dm755 pacs2repo-gui "$pkgdir/usr/bin/pacs2repo-gui"
    install -Dm644 pacs2repo.1.gz "$pkgdir/usr/share/man/man1/pacs2repo.1.gz"
    install -Dm644 pacs2repo.1.gz "$pkgdir/usr/share/man/man1/pacs2repo-gui.1.gz"
}
