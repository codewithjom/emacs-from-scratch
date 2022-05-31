# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: Jom Dollesin <codewithjom@gmail.com>
pkgname=jdos-emacs-git
pkgver=28.1.r1.0fa5ae7
pkgrel=1
epoch=
pkgdesc="JDOS emacs-from-scratch configuration."
arch=('x86_64')
url="https://github.com/codewithjom/emacs-from-scratch.git"
license=('GPL3')
groups=()
depends=('emacs' 'ripgrep' 'ttf-jetbrains-mono' 'ttc-iosevka-aile')
makedepends=('git')
checkdepends=()
optdepends=()
provides=(emacs)
conflicts=(emacs)
replaces=()
backup=()
options=()
install=
changelog=
source=("git+$url")
noextract=()
md5sums=('SKIP')
validpgpkeys=()

pkgver() {
	cd "${_pkgver}"
	printf "28.1.r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

# build() {
# 	cd "$srcdir/jdos-emacs-git"
# 	make X11INC=/usr/include/X11 X11LIB=/usr/lib/X11
# 
# 	local _conf=(
# 	  --prefix=/usr
# 		--sysconfdir=/etc
# 		--libexecdir=/usr/lib
# 		--localstatedir=/var
# 		--mandir=/usr/share/man
# 		--with-gameuser=:games
# 		--with-modules
# 		--without-libotf
# 		--without-m17n-flt
# 		--without-gconf
# 		--without-gsettings
# 	)
# }
# 
# package() {
# 	cd "$pkgdir/jdos-emacs-git/build"
# 	mkdir -p ${pkgdir}/opt/${pkgname}
# 	cp -rf * ${pkgdir}/opt/${pkgname}
# 	make PREFIX=/usr DESTDIR="${pkgdir}" install
# 	install -Dm644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
# 	install -Dm644 README.md "{pkgdir}/usr/share/doc/${pkgname}/README.md"
# }
