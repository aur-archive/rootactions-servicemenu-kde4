# Maintainer: Antonio Rojas < nqn1976 @ gmail.com >
# Contributor: Jan Valiska <jan.valiska@gmail.com>

pkgname=rootactions-servicemenu-kde4
pkgver=2.7.3
pkgrel=1
pkgdesc="Allows admin users to perform several root only actions from dolphin via kdesu/kdesudo"
arch=('any')
url="http://www.kde-apps.org/content/show.php?content=48411"
license=('GPL')
depends=('kdebase-dolphin' 'kdeutils-ark')
source=("http://www.kde-apps.org/CONTENT/content-files/48411-rootactions_servicemenu_$pkgver.tar.gz")
md5sums=('f887ebb733b5853ef8b583da6677bc8a')

package() {
cd $srcdir/rootactions_servicemenu_$pkgver/Root_Actions_$pkgver/dolphin-KDE4/
mkdir -p $pkgdir/usr/share/kde4/services/ServiceMenus/
install -m755 *.desktop $pkgdir/usr/share/kde4/services/ServiceMenus/
cd $srcdir/rootactions_servicemenu_$pkgver/Root_Actions_$pkgver 
install -Dm755 rootactions-servicemenu.pl $pkgdir/usr/bin/rootactions-servicemenu.pl
} 
