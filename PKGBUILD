# Contributor: Aakos <scooterbr at gmail dot com>

pkgname="gamcat"
pkgver="1.0.5"
pkgrel=1
debrel=1
pkgdesc="Gamcat - CD/DVD catalog software"
arch=('any')
url="http://www.kde-apps.org/content/show.php/GamCat?content=100682"
license=('GPL')
depends=('gambas3-runtime' 'gambas3-gb-qt4' 'gambas3-gb-form' 'gambas3-gb-form-stock' 'gambas3-gb-db' 'gambas3-gb-db-form' 'gambas3-gb-db-sqlite3' 'gambas3-gb-desktop' 'gambas3-gb-net' 'gambas3-gb-net-curl' 'gambas3-gb-net-smtp' 'gambas3-gb-report' 'gambas3-gb-media')
optdepends=('cdrkit' 'imagemagick' 'unrar' 'unzip' 'unace' 'unarj')
source=("http://downloads.sourceforge.net/project/gamcat/gamcat-${pkgver}/gamcat_${pkgver}-${debrel}_all.deb")

md5sums=('1c8d83090c7f34af7060522ed83e71c6')


build()
{
	cd ${srcdir}
	ar x ${pkgname}_${pkgver}-${debrel}_all.deb
	tar -zxf data.tar.gz
	rm -rf ${srcdir}/usr/share/menu
	mkdir ${pkgdir}/usr
	cd ${srcdir}/usr
	cp -r bin ${pkgdir}/usr
	cp -r share ${pkgdir}/usr
}
