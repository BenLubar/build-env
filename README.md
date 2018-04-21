# DFHack Build Environment

*Currently, this does not support Windows builds. I'm trying to fix that. You can see my progress here: <https://what.thedailywtf.com/post/1337023>*

## Contents

- Ubuntu Bionic (18.04 LTS)
- buildpack-deps (see [Docker Hub](https://hub.docker.com/_/buildpack-deps/) description for details)
- GNU C/C++ compilers (gcc and g++)
  - Versions: 4.8.5 and 7.3.0 (or later)
  - Linux: 32-bit and 64-bit
  - Mac OS X: 32-bit and 64-bit, minimum version OS X 10.6
- ccache (intended to have cache directory stored outside the container)
- CMake version 3.10 or later
- Google protocol buffer compiler (shim DFHack native build directory at `/home/buildmaster/dfhack-native`)
- Perl with `XML::LibXML` and `XML::LibXSLT` (required for df-structures)
- OpenGL headers and libraries (required for Stonesense)
- Sphinx (used to build DFHack documentation)
- zlib for 32- and 64-bit Linux and Mac OS X

## Special Thanks

- Mac OS X cross-compiler: <https://github.com/tpoechtrager/osxcross>
- Mac OS X SDK mirror: <https://github.com/phracker/MacOSX-SDKs>
