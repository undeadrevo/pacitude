# Maintainer: Abraham Levine <echo iue@trnspljc.890 | tr ietursnpl890jc acprlsurecomed>

pkgname=pacitude
pkgver=1.0
pkgrel=1
pkgdesc="a pacman/pacaur wrapper with apt inspired syntax"
arch=('i686' 'x86_64')
url="https://git.shittyne.ws/sachikos/pacitude.git"
license=('WTFPL')
depends=('sudo' 'pacaur' 'cower')
makedepends=('git')
source=('git://git.shittyne.ws/sachikos/pacitude.git')
md5sums=('SKIP')

pkgver() {
        cd "$_gitname" &&
        printf '%s.%s\n' "$(git rev-list --count HEAD)" \
                         "$(git rev-parse --short HEAD)"
}

package() {
        cd "$_gitname" &&
        install -m 755 -D pacitude "$pkgdir/usr/bin/pacitude"
}
