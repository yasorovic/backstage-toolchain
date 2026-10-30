# Backstage toolchain mirror

Copies of the pacman packages that the Backstage installer needs to build a GBA ROM
(devkitARM, libgba, maxmod, grit, mmutil and the tools of devkitPro, plus make, sh, mkdir and rm from MSYS2
on Windows). They are mirrored here because the official servers sometimes refuse automated downloads and
drop old versions. Backstage downloads them from this release and checks each SHA-256 (listed in `SHA256SUMS`)
before installing anything. 

Nothing here is modified.

Each package keeps its own license, shipped inside the archive (`licenses/` for devkitPro,
`usr/share/licenses/` for MSYS2). Sources: devkitPro packages are built from
https://github.com/devkitPro/pacman-packages (each recipe points to the upstream source of the exact version);
MSYS2 packages are built from https://github.com/msys2/MSYS2-packages. No BIOS or Nintendo content is included.

| Package | Version | Platform | Asset | Official origin |
| --- | --- | --- | --- | --- |
| devkitarm-gcc | 16.1.0-1 | windows | windows-devkitarm-gcc-16.1.0-1-x86_64.pkg.tar.zst | https://pkg.devkitpro.org/packages/windows/x86_64/devkitarm-gcc-16.1.0-1-x86_64.pkg.tar.zst |
| devkitarm-binutils | 2.46.0-1 | windows | windows-devkitarm-binutils-2.46.0-1-x86_64.pkg.tar.zst | https://pkg.devkitpro.org/packages/windows/x86_64/devkitarm-binutils-2.46.0-1-x86_64.pkg.tar.zst |
| devkitarm-newlib | 4.6.0.20260123-5 | any | devkitarm-newlib-4.6.0.20260123-5-any.pkg.tar.zst | https://pkg.devkitpro.org/packages/devkitarm-newlib-4.6.0.20260123-5-any.pkg.tar.zst |
| devkitarm-crtls | 1.2.6-1 | any | devkitarm-crtls-1.2.6-1-any.pkg.tar.zst | https://pkg.devkitpro.org/packages/devkitarm-crtls-1.2.6-1-any.pkg.tar.zst |
| devkitarm-rules | 1.6.0-4 | any | devkitarm-rules-1.6.0-4-any.pkg.tar.zst | https://pkg.devkitpro.org/packages/devkitarm-rules-1.6.0-4-any.pkg.tar.zst |
| libgba | 0.5.4-1 | any | libgba-0.5.4-1-any.pkg.tar.zst | https://pkg.devkitpro.org/packages/libgba-0.5.4-1-any.pkg.tar.zst |
| maxmod-gba | 1.0.15-1 | any | maxmod-gba-1.0.15-1-any.pkg.tar.xz | https://pkg.devkitpro.org/packages/maxmod-gba-1.0.15-1-any.pkg.tar.xz |
| grit | 0.10.0-1 | windows | windows-grit-0.10.0-1-x86_64.pkg.tar.zst | https://pkg.devkitpro.org/packages/windows/x86_64/grit-0.10.0-1-x86_64.pkg.tar.zst |
| mmutil | 1.10.1-1 | windows | windows-mmutil-1.10.1-1-x86_64.pkg.tar.xz | https://pkg.devkitpro.org/packages/windows/x86_64/mmutil-1.10.1-1-x86_64.pkg.tar.xz |
| general-tools | 1.4.4-1 | windows | windows-general-tools-1.4.4-1-x86_64.pkg.tar.zst | https://pkg.devkitpro.org/packages/windows/x86_64/general-tools-1.4.4-1-x86_64.pkg.tar.zst |
| gba-tools | 1.2.0-2 | windows | windows-gba-tools-1.2.0-2-x86_64.pkg.tar.xz | https://pkg.devkitpro.org/packages/windows/x86_64/gba-tools-1.2.0-2-x86_64.pkg.tar.xz |
| msys2-runtime | 3.6.11-4 | msys2 | msys2-msys2-runtime-3.6.11-4-x86_64.pkg.tar.zst | https://repo.msys2.org/msys/x86_64/msys2-runtime-3.6.11-4-x86_64.pkg.tar.zst |
| bash | 5.3.20-2 | msys2 | msys2-bash-5.3.20-2-x86_64.pkg.tar.zst | https://repo.msys2.org/msys/x86_64/bash-5.3.20-2-x86_64.pkg.tar.zst |
| make | 4.4.1-2 | msys2 | msys2-make-4.4.1-2-x86_64.pkg.tar.zst | https://repo.msys2.org/msys/x86_64/make-4.4.1-2-x86_64.pkg.tar.zst |
| coreutils | 8.32-5 | msys2 | msys2-coreutils-8.32-5-x86_64.pkg.tar.zst | https://repo.msys2.org/msys/x86_64/coreutils-8.32-5-x86_64.pkg.tar.zst |
| libintl | 0.22.5-1 | msys2 | msys2-libintl-0.22.5-1-x86_64.pkg.tar.zst | https://repo.msys2.org/msys/x86_64/libintl-0.22.5-1-x86_64.pkg.tar.zst |
| libiconv | 1.18-1 | msys2 | msys2-libiconv-1.18-1-x86_64.pkg.tar.zst | https://repo.msys2.org/msys/x86_64/libiconv-1.18-1-x86_64.pkg.tar.zst |
| gcc-libs | 13.4.0-1 | msys2 | msys2-gcc-libs-13.4.0-1-x86_64.pkg.tar.zst | https://repo.msys2.org/msys/x86_64/gcc-libs-13.4.0-1-x86_64.pkg.tar.zst |
| devkitarm-gcc | 16.1.0-1 | linux | linux-devkitarm-gcc-16.1.0-1-x86_64.pkg.tar.zst | https://pkg.devkitpro.org/packages/linux/x86_64/devkitarm-gcc-16.1.0-1-x86_64.pkg.tar.zst |
| devkitarm-binutils | 2.46.0-1 | linux | linux-devkitarm-binutils-2.46.0-1-x86_64.pkg.tar.zst | https://pkg.devkitpro.org/packages/linux/x86_64/devkitarm-binutils-2.46.0-1-x86_64.pkg.tar.zst |
| grit | 0.10.0-1 | linux | linux-grit-0.10.0-1-x86_64.pkg.tar.zst | https://pkg.devkitpro.org/packages/linux/x86_64/grit-0.10.0-1-x86_64.pkg.tar.zst |
| mmutil | 1.10.1-1 | linux | linux-mmutil-1.10.1-1-x86_64.pkg.tar.xz | https://pkg.devkitpro.org/packages/linux/x86_64/mmutil-1.10.1-1-x86_64.pkg.tar.xz |
| general-tools | 1.4.4-1 | linux | linux-general-tools-1.4.4-1-x86_64.pkg.tar.zst | https://pkg.devkitpro.org/packages/linux/x86_64/general-tools-1.4.4-1-x86_64.pkg.tar.zst |
| gba-tools | 1.2.0-1 | linux | linux-gba-tools-1.2.0-1-x86_64.pkg.tar.xz | https://pkg.devkitpro.org/packages/linux/x86_64/gba-tools-1.2.0-1-x86_64.pkg.tar.xz |
