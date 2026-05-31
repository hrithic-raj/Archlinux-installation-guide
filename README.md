[hrj@HRJ caelestia]$ paru -S caelestia-shell
:: Resolving dependencies...
:: There are 2 providers available for caelestia-shell:
:: Repository AUR:
    1) caelestia-shell  2) caelestia-shell-git  
Enter a number (default=1): 2
:: Calculating conflicts...
:: Calculating inner conflicts...

Aur (1) caelestia-shell-git-1.2.0.r0.g2bd7089-2

:: Proceed to review? [Y/n]: y

:: Downloading PKGBUILDs...
 (1/1) caelestia-shell-git-1.2.0.r0.g2bd7089-2       [---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------]
:: caelestia-shell-git:
  PKGBUILD:
    # caelestia-shell
    
    # Maintainer: Soramane <soramane32 at gmail dot com>
    
    _pkgname='caelestia-shell'
    pkgname="$_pkgname-git"
    pkgver=1.2.0.r0.g2bd7089
    pkgrel=2
    pkgdesc='The desktop shell for the Caelestia dotfiles'
    arch=('x86_64')
    url='https://github.com/caelestia-dots/shell'
    license=('GPL-3.0-only')
    depends=('caelestia-cli' 'quickshell-git' 'ddcutil' 'brightnessctl' 'app2unit' 'libcava' 'networkmanager'
             'lm_sensors' 'fish' 'aubio' 'libpipewire' 'glibc' 'gcc-libs' 'ttf-material-symbols-variable' 'power-profiles-daemon'
             'ttf-rubik-vf' 'ttf-cascadia-code-nerd' 'swappy' 'libqalculate' 'bash' 'qt6-base' 'qt6-declarative')
    makedepends=('git' 'cmake' 'ninja')
    provides=($_pkgname)
    conflicts=($_pkgname)
    source=("$pkgname::git+$url.git")
    sha256sums=('SKIP')
    
    pkgver() {
        cd "${srcdir}/${pkgname}"
        git describe --long --tags --abbrev=7 | sed 's/^v//;s/\([^-]*-g\)/r\1/;s/-/./g'
    }
    
    build() {
        cd "${srcdir}/${pkgname}"
    
        cmake -B build -G Ninja -DCMAKE_BUILD_TYPE=RelWithDebInfo -DCMAKE_INSTALL_PREFIX=/ -DDISTRIBUTOR="AUR (package: $pkgname)"
        cmake --build build
    }
    
    package() {
        cd "${srcdir}/${pkgname}"
    
        DESTDIR="$pkgdir" cmake --install build
        install -Dm644 LICENSE "$pkgdir"/usr/share/licenses/$_pkgname/LICENSE
    }

:: Accept changes? [Y/n]: y
fetching devel info...
==> Making package: caelestia-shell-git 1.2.0.r0.g2bd7089-2 (Sun 31 May 2026 02:06:32 PM IST)
==> Retrieving sources...
  -> Cloning caelestia-shell-git git repo...
Cloning into bare repository '/home/hrj/.cache/paru/clone/caelestia-shell-git/caelestia-shell-git'...
remote: Enumerating objects: 34078, done.
remote: Counting objects: 100% (2091/2091), done.
remote: Compressing objects: 100% (445/445), done.
remote: Total 34078 (delta 1878), reused 1655 (delta 1645), pack-reused 31987 (from 3)
Receiving objects: 100% (34078/34078), 27.35 MiB | 4.69 MiB/s, done.
Resolving deltas: 100% (24233/24233), done.
==> Validating source files with sha256sums...
    caelestia-shell-git ... Skipped
==> Making package: caelestia-shell-git 1.2.0.r0.g2bd7089-2 (Sun 31 May 2026 02:06:41 PM IST)
==> Checking runtime dependencies...
==> Checking buildtime dependencies...
==> Retrieving sources...
  -> Updating caelestia-shell-git git repo...
==> Validating source files with sha256sums...
    caelestia-shell-git ... Skipped
==> Removing existing $srcdir/ directory...
==> Extracting sources...
  -> Creating working copy of caelestia-shell-git git repo...
Cloning into 'caelestia-shell-git'...
done.
==> Starting pkgver()...
==> Updated version: caelestia-shell-git 1.6.2.r12.g63bb827-1
==> Sources are ready.
caelestia-shell-git-1.2.0.r0.g2bd7089-2: parsing pkg list...
==> Making package: caelestia-shell-git 1.6.2.r12.g63bb827-1 (Sun 31 May 2026 02:06:43 PM IST)
==> Checking runtime dependencies...
==> Checking buildtime dependencies...
==> WARNING: Using existing $srcdir/ tree
==> Starting pkgver()...
==> Starting build()...
-- The CXX compiler identification is GNU 16.1.1
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /usr/bin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD - Success
-- Found Threads: TRUE
-- Could NOT find Qt6ShaderTools (missing: Qt6ShaderTools_DIR)
CMake Error at plugin/src/Caelestia/CMakeLists.txt:1 (find_package):
  Found package configuration file:

    /usr/lib/cmake/Qt6/Qt6Config.cmake

  but it set Qt6_FOUND to FALSE so package "Qt6" is considered to be NOT
  FOUND.  Reason given by package:

  Failed to find required Qt component "ShaderTools".

  Expected Config file at
  "/usr/lib/cmake/Qt6ShaderTools/Qt6ShaderToolsConfig.cmake" does NOT exist



  Configuring with --debug-find-pkg=Qt6ShaderTools might reveal details why
  the package was not found.

  Configuring with -DQT_DEBUG_FIND_PACKAGE=ON will print the values of some
  of the path variables that find_package uses to try and find the package.



-- Configuring incomplete, errors occurred!
==> ERROR: A failure occurred in build().
    Aborting...
error: failed to build 'caelestia-shell-git-1.2.0.r0.g2bd7089-2': 
error: packages failed to build: caelestia-shell-git-1.2.0.r0.g2bd7089-2
[hrj@HRJ caelestia]$ 
