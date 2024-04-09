# Maintainer: Andrii Burkivskyi <aburkivskyi@outlook.com>

pkgname="find-the-command"
pkgver=2.0.1
pkgrel=1
pkgdesc="find-the-command for termux-pacman"
arch=('any')
url="https://github.com/aburkivskyi/find-the-command"
license=('custom:WTFPL')
depends=('pacman')
optdepends=('fzf' 'pkgfile')
makedepends=('git')
#source=("usr")
#sha256sums=('SKIP')

#pkgver() {
#	printf "r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
#}

package() {
	cd "${startdir}"
	install -Dm644 "usr/share/doc/find-the-command/ftc.bash" "${terdir}/usr/share/doc/find-the-command/ftc.bash"
	install -Dm644 "usr/share/doc/find-the-command/ftc.zsh" "${terdir}/usr/share/doc/find-the-command/ftc.zsh"
	install -Dm644 "usr/share/doc/find-the-command/ftc.fish" "${terdir}/usr/share/doc/find-the-command/ftc.fish"
	install -Dm644 "LICENSE" "${terdir}/usr/share/licenses/${pkgname}/LICENSE"
}
