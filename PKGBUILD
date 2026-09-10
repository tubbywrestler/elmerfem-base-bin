# Maintainer: pineappletoad

pkgname=elmerfem-base-bin
pkgver=26.2.1
_pkgrel_src=2
pkgrel=1
pkgdesc="A finite element software for multiphysical problems (without GUI and Ice, precompiled)"
arch=('x86_64')
url="https://www.elmerfem.org"
license=('GPL-2.0-only AND LGPL-2.1-only AND LicenseRef-Elmer')
options=('!debug')
provides=('elmerfem-base')
conflicts=('elmerfem-base' 'elmerfem-git' 'elemerfem')
depends=(
    'arpack'
    'blas-openblas'
    'hypre'
    'openmp'
    'openmpi'
)

source=("https://github.com/tubbywrestler/elmerfem-base-bin/releases/download/${pkgver}-${_pkgrel_src}/elmerfem-base-${pkgver}-${_pkgrel_src}-x86_64.pkg.tar.zst")
sha256sums=('df37a1246fabad5141b315ff8b86aa914de39c2b233bdcc3c894ca31b8ce276a')

package() {
    bsdtar -xf "${srcdir}/elmerfem-base-${pkgver}-${_pkgrel_src}-x86_64.pkg.tar.zst" -C "${pkgdir}" --exclude .PKGINFO --exclude .BUILDINFO --exclude .MTREE
}
