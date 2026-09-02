# Maintainer: piratecarrot

pkgname=elmerfem-base-bin
pkgver=26.2.1
_pkgrel_src=1
pkgrel=1
pkgdesc="A finite element software for multiphysical problems (without GUI and Ice, precompiled)"
arch=('x86_64')
url="https://www.elmerfem.org"
license=('GPL-2.0-only AND LGPL-2.1-only AND LicenseRef-Elmer')
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
sha256sums=('bc0837706741633165e925f93e5c7541f3810628657882f86ef0524a3f36b0fd')

package() {
    bsdtar -xf "${srcdir}/elmerfem-base-${pkgver}-${_pkgrel_src}-x86_64.pkg.tar.zst" -C "${pkgdir}" --exclude .PKGINFO --exclude .BUILDINFO --exclude .MTREE
}
