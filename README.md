Reverse
=======

Reverse engineering for x86 binaries. Generate a more readable code (pseudo-C)
with colored syntax.

Supported formats :
    `ELF`
    `PE` : no symbol resolution for the moment


The `Makefile` is used only for checking tests.


## Requirements

    python3
    python-capstone (>= 3.0.1)
    python-pyelftools
    https://github.com/simonzack/pefile-py3k
    terminal with 256 colors (if not use the option `--nocolor`)

For Python binding of [Capstone engine](http://www.capstone-engine.org), you 
can install it from PyPi, like followings: 

    sudo pip3 install capstone


## Example

    $ ./reverse.py tests/nestedloop1.bin

![reverse](http://hippersoft.fr/projects/rev.jpg)


By opening `d3/index.html` (with the option `--graph`) you will be able to
see the flow graph :

![graph](http://hippersoft.fr/projects/graph.jpg)

