# libelectronpass
[![Build Status](https://travis-ci.org/electronpass/libelectronpass.svg?branch=release)](https://travis-ci.org/electronpass/libelectronpass)

Backend for electronpass-desktop that can work with the wallet format writen in c++.

## Dependencies

- [libsodium](https://libsodium.org) - A modern and easy-to-use crypto library
- [jsoncpp v1.8.0](https://github.com/open-source-parsers/jsoncpp) - Already included in source code
- [gtest](https://github.com/google/googletest) - Required for building tests. Already included in source code
- [doxygen](http://www.stack.nl/~dimitri/doxygen/) - Required for building documentation

## Building
CMake configuration is used to create documentation and run tests.

The following will build examples and tests

    mkdir build; cd build
    cmake ..
    make -j8

## Tests
You can run the tests with

```make check```

You can also compile and run the tests with

```
make tests
./bin/tests
```

## Documentation
Documentation is generated using doxygen:

    doxygen docs/Doxyfile


You can also use make to generate documentation with:

    make docs

## Examples
Simple usage examples are located in ```examples/``` folder. To build all examples run from ```build/``` folder:

    make examples

## License
Code in this project is licensed under [GNU LGPLv3 license](https://github.com/electronpass/libelectronpass/blob/release/LICENSE.LESSER). Some third party files are subjective to their respective license.

### JsonCpp
[JsonCpp](https://github.com/open-source-parsers/jsoncpp) is licensed under the MIT license. Used files are:

- ```include/json/*```
- ```src/jsoncpp.cpp```
