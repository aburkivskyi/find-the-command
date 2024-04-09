# Maintainer: Andrii Burkivskyi <aburkivskyi@outlook.com>

pkgname="find-the-command"
pkgver=2.0.2
pkgrel=1
pkgdesc="find-the-command for termux-pacman"
arch=('any')
url="https://github.com/aburkivskyi/find-the-command"
license=('custom:WTFPL')
depends=('pacman>=5.0')
optdepends=('fzf' 'pkgfile')
options=('docs')
install=find-the-command.install

package() {
	cd "${startdir}"
	install -Dm644 README.md "usr/share/doc/${pkgname}"/ftc.* -t \
		"${terdir}/usr/share/doc/${pkgname}"
	install -Dm644 LICENSE -t "${terdir}/usr/share/licenses/${pkgname}"
}
