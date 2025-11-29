[![MacOS Build for GNU Emacs](https://github.com/RadioNoiseE/ebuild/actions/workflows/build.yml/badge.svg)](https://github.com/RadioNoiseE/ebuild/actions/workflows/build.yml)

This repository automatically builds GNU Emacs with the Memory Pool
System for Darwin every day at UTC 0:00, directly from upstream git
sources. This build is intended for Emacs developers who want to test
the bleeding-edge version. Please report any bugs directly to the
Emacs mailing list, as the source is not modified here.

No package manager is used during the build process, as all external
dependencies are fetched from upstream and compiled from source. A
statically linked Emacs is produced (except the system components).

> [!Note]
> Emacs is built with the GNU MP Bignum Library, GnuTLS, Tree Sitter,
> XML2 and Zlib.  Native compilation is likely not supported, since
> compiling libgccjit is considered too resource-intensive, and it
> will probably take hours to generate native components after temacs
> bootstrap.
