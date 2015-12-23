
# conan-libxml2

[Conan.io](https://conan.io) package for libxml2 library

The packages generated with this **conanfile** can be found in [conan.io](https://conan.io/source/libxml2/2.9.3/lasote/stable).

## Build packages

Download conan client from [Conan.io](https://conan.io) and run:

    $ python build.py
    
## Upload packages to server

    $ conan upload libxml2/2.9.3@lasote/stable --all
    
## Reuse the packages

### Basic setup

    $ conan install libxml2/2.9.3@lasote/stable
    
### Project setup

If you handle multiple dependencies in your project is better to add a *conanfile.txt*
    
    [requires]
    libxml2/2.9.3@lasote/stable

    [options]
    libxml2:shared=true # false
    
    [generators]
    txt
    cmake

Complete the installation of requirements for your project running:</small></span>

    conan install . 

Project setup installs the library (and all his dependencies) and generates the files *conanbuildinfo.txt* and *conanbuildinfo.cmake* with all the paths and variables that you need to link with your dependencies.
