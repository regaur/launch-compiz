# Maintainer: Jan Boelsche <jan@lagomorph.de>

pkgname='launch-compiz'
pkgver=1.1
pkgrel=1
pkgdesc='Start compiz in the background when auto-login xsession starts'
packager='Jan Boelsche'
arch=('any')
license=('GPL')
groups=()
depends=(
  'lightdm-autologin'
  'ccsm'
)
makedepends=()
checkdepends=()
optdepends=()

source=(
  '10-launch-compiz'
)

sha256sums=('1ccf123b2ea6b3ef932784d82b2ca702b7ac1e0227afbb345eda17ac2addffb9')

package() {
  home=${pkgdir}/home/auto-login
	install -m 755 -d "${home}/xsession.d"
	install -m 755 -t "${home}/xsession.d" '10-launch-compiz'
}

