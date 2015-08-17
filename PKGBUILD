# Maintainer: Pantelis Panayiotou <p.panayiotou@gmail.com>
pkgname=operprinting-ppds-postscript-ricoh
pkgver=20140829
pkgrel=1
pkgdesc="PPD files for Ricoh's PostScript printers, supplied by Ricoh"
arch=('any')
url='https://www.openprinting.org/driver/Postscript-Ricoh'
license=('MIT')
depends=(cups ghostscript)
conflicts=(ppd-ricoh)
install=driver.install
source=('https://www.openprinting.org/download/printdriver/components/lsb3.2/main/RPMS/noarch/openprinting-ppds-postscript-ricoh-20140829-1lsb3.2.noarch.rpm')
md5sums=('ebde805445988d13c39fe111ef256d0c')

package() {
  install -d $pkgdir/usr/share/cups/model/Ricoh $pkgdir/usr/share/doc/ricoh-postscript
  install $srcdir/opt/OpenPrinting-Ricoh/ppds/Ricoh/* $pkgdir/usr/share/cups/model/Ricoh/
  install $srcdir/opt/OpenPrinting-Ricoh/doc/openprinting-ppds-postscript-ricoh/* $pkgdir/usr/share/doc/ricoh-postscript/
}
