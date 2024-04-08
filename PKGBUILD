# Maintainer: Andrii Burkivskyi <aburkivskyi@outlook.com>

pkgname="find-the-command"
pkgver=r98.7d7e0b6
pkgrel=1
pkgdesc="find-the-command for termux-pacman"
arch=('any')
url="https://github.com/aburkivskyi/find-the-command"
license=('custom:WTFPL')
depends=('pacman')
optdepends=('fzf' 'pkgfile')
makedepends=('git')
source=("git+https://github.com/aburkivskyi/find-the-command")
sha256sums=('SKIP')

pkgver() {
	cd "${pkgname}"
	printf "r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

package() {
	cd "${pkgname}"
	install -Dm600 "usr/share/doc/find-the-command/ftc.bash" "${terdir}/usr/share/doc/find-the-command/ftc.bash"
	install -Dm600 "usr/share/doc/find-the-command/ftc.zsh" "${terdir}/usr/share/doc/find-the-command/ftc.zsh"
	install -Dm600 "usr/share/doc/find-the-command/ftc.fish" "${terdir}/usr/share/doc/find-the-command/ftc.fish"
	install -Dm600 "LICENSE" "${terdir}/usr/share/licenses/${pkgname}/LICENSE"
}