# Maintainer: Diamond Bond <diamondbond1@gmail.com>
# This PKGBUILD needs an rpm downloaded from https://account.wolfram.com/products/downloads/wolframscript
# placed in the same directory

pkgname=wolframscript
pkgver=13.0.0
pkgrel=1
pkgdesc="Execute Wolfram Language Code Anywhere"
arch=('x86_64')
url="https://www.wolfram.com/wolframscript/"
license=('proprietary')
source=("local://WolframScript_${pkgver}_LINUX64_x86_64.rpm")
conflicts=('mathematica')
# The conflict arises due to some files that both packages use.
# If you would like both installed, install the generated .tar.xz --overwrite '*' 
md5sums=('02568cd6d08c8c538360106eac2fe967')

package() {
  cd "${srcdir}"
  install -Dm 0755 opt/Wolfram/WolframScript/bin/wolframscript -t "${pkgdir}"/usr/bin/
  install -D opt/Wolfram/WolframScript/man/man1/wolframscript.1 -t "${pkgdir}"/usr/share/man/man1
  cp -r usr/share/* "${pkgdir}"/usr/share/
}

