[![Download](https://api.bintray.com/packages/slepasteur/public-conan/immer%3Aslepasteur/images/download.svg) ](https://bintray.com/slepasteur/public-conan/immer%3Aslepasteur/_latestVersion)
[![Build Status Travis](https://travis-ci.org/slepasteur/conan-immer.svg?branch=testing%2F0.4.0)](https://travis-ci.org/slepasteur/conan-immer)
[![Build Status AppVeyor](https://ci.appveyor.com/api/projects/status/github/slepasteur/conan-immer?branch=testing%2F0.4.0&svg=true)](https://ci.appveyor.com/project/slepasteur/conan-immer)

## Conan package recipe for [*immer*](https://github.com/arximboldi/immer)

Postmodern immutable and persistent data structures for C++

The packages generated with this **conanfile** can be found on [Bintray](https://bintray.com/slepasteur/public-conan/immer%3Aslepasteur).


## Issues

If you wish to report an issue or make a request for a Bincrafters package, please do so here:

[Bincrafters Community Issues](https://github.com/bincrafters/community/issues)


## For Users

### Basic setup

    $ conan install immer/0.4.0@slepasteur/testing

### Project setup

If you handle multiple dependencies in your project is better to add a *conanfile.txt*

    [requires]
    immer/0.4.0@slepasteur/testing

    [generators]
    txt

Complete the installation of requirements for your project running:

    $ mkdir build && cd build && conan install ..

Note: It is recommended that you run conan install from a build directory and not the root of the project directory.  This is because conan generates *conanbuildinfo* files specific to a single build configuration which by default comes from an autodetected default profile located in ~/.conan/profiles/default .  If you pass different build configuration options to conan install, it will generate different *conanbuildinfo* files.  Thus, they should not be added to the root of the project, nor committed to git.


## Build and package

The following command both runs all the steps of the conan file, and publishes the package to the local system cache.  This includes downloading dependencies from "build_requires" and "requires" , and then running the build() method.

    $ conan create . slepasteur/testing




## Add Remote

    $ conan remote add slepasteur "https://api.bintray.com/conan/slepasteur/public-conan"


## Conan Recipe License

NOTE: The conan recipe license applies only to the files of this recipe, which can be used to build and package immer.
It does *not* in any way apply or is related to the actual software being packaged.

[MIT](https://github.com/slepasteur/conan-immer/blob/testing/0.4.0/LICENSE.md)
