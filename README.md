# MuPDF prebuilt libraries

Made for my tool that depends on mupdf: [pymupdf4llm-C](https://github.com/intercepted16/pymupdf4llm-C). Artifex didn't seem to give links for MUPDF shared libraries, despite bundling them in PyMUPDF and others. A bit odd. But here we are.

You can find them in the Releases page. There are Linux, macOS, and Windows builds.
It uses a GitHub action, which is in `.github/workflows/build.yml`.

- supports Linux (x86_64), macOS ARM, and Windows x86_64.

- Uses `manylinux2014` (has an older `glibc` version) so that pretty much all modern Linux distributions are supported

- all M* series chips should work for macOS builds
- Windows builds are produced with MSYS2 MinGW/UCRT and publish `libmupdf.dll` plus `libmupdf.dll.a`.
