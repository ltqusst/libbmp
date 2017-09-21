# libbmp
a clone from envyen's libbmp, with building system replaced by cmake

Usage:

    mkdir build
    cmake ../src/
    make
    sudo make install

default install location is /usr/local/lib & include, so make sure prefix your exe with LD_LIBRARY_PATH=/usr/local/lib when invoking from commmand line.
