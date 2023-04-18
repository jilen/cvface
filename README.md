# Opencv based face lib(jni build)

A custom build of opencv 4.7.0 with objdetect, dnn (used for face recoginition).

# Build requirements

* CMake 3.3 +
* CXX 17 compatible toolchain
* Opencv required libs

# Build instructions
+ Run `gen-src.sh` generate the dynamic lib and java source into the `cvface/src/gen` folder.
+ Run `gradle build` in `cvface` fold to build jar.


# What's changed ?

* Only face recoginition related modules are build.
* Build fat lib (single shared library) by default.
* Provide simply facility load library and convert `BufferedImage` to `Mat`
* Removed `finalize`, resource should be released manually.
