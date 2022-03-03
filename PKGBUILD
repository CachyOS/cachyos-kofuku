# Maintainer: Vladislav Nepogodin <nepogodin.vlad@gmail.com>

pkgname=cachyos-kofuku
pkgver=1.0.0
pkgrel=1
arch=('any')
url="https://github.com/cachyos/$pkgname"
license=('MIT')
makedepends=('coreutils')
source=("$pkgname-$pkgver.tar.gz::$url/archive/v$pkgver.tar.gz")
sha256sums=('SKIP')
pkgdesc='Kofuku settings'
depends=('cachyos-zsh-config'
        'nerd-fonts-fantasque-sans-mono'
        'rofi'
        'rxvt-unicode'
        'lightdm-webkit2-greeter'
        'picom'
        'polybar'
        'sxhkd'
        'deadd-notification-center'
        'ttf-fira-sans')
install=$pkgname.install
provides=('cachyos-desktop-settings')
conflicts=('cachyos-desktop-settings' 'lightdm-webkit2-theme-glorious')

package() {
    install -d $pkgdir/etc
    cp -rf $srcdir/$pkgname-$pkgver/etc $pkgdir
    install -d $pkgdir/usr
    cp -rf $srcdir/$pkgname-$pkgver/usr $pkgdir
}
