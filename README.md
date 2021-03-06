# Core

## Introduction

Core provides the functionality necessary to couple the individual SCINE
modules together. It is vital for the correct functioning of all SCINE
modules, but it does not directly provide any functionality for end users.
Therefore, only developers of SCINE need to directly interact with Core.


## License and Copyright Information

For license and copyright information, see the file `LICENSE.txt` in this
directory.


## Installation and Usage

As a user of one of the SCINE modules (such as Sparrow), you do not need
to set up Core yourself. Instead, this is done as part of the installation
process of the respective SCINE module. Therefore, the following instructions
are only necessary for developers of SCINE, or those implementing the 
interfaces defined here.

### Dependencies

- cmake (at least version 3.9.0)
- A C++ compiler supporting the C++14 standard (we recommend GCC 7.3.0)
- The Boost libraries (we recommend version 1.64.0)

### Installation

In order to compile this as a SCINE developer, execute the following
commands:

```
git submodule init
git submodule update
mkdir build inst
cd build
cmake -DCMAKE_BUILD_TYPE=Release -DCMAKE_INSTALL_PREFIX=../inst ..
make -j 4
make CoreDocumentation
make install
```


## Support and Contact

In case you should encounter problems or bugs, please write a short message
to scine@phys.chem.ethz.ch.

