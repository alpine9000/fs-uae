1. gcc osx (if you don't have gcc)
    cd downloads
    curl -OL http://mirrors.concertpass.com/gcc/releases/gcc-6.3.0/gcc-6.3.0.tar.gz
    cd ../builds
    tar zxfv ../downloads/gcc-6.3.0.tar.gz
    cd gcc-6.3.0
    ./contrib/download_prerequisites
    cd ..
    mkdir gcc-6.3.0.build
    cd gcc-6.3.0.build
    ../gcc-6.3.0/configure --prefix=/usr/local/ --enable-languages=c,c++
    make -j4
    make install
    cd ../../
```

2. SDL 2.0.5
    ```
    cd downloads
    curl -OL https://www.libsdl.org/release/SDL2-2.0.5.tar.gz
    cd ../build
    tar zxfv ../downloads/SDL2-2.0.5.tar.gz
    cd SDL2-2.0.5
    ./configure --prefix=/usr/local CC=clang
    make -j4
    make install
    cd ../..
```

3. pkg-config
    ```
    cd downloads 
    curl -OL https://pkg-config.freedesktop.org/releases/pkg-config-0.29.tar.gz
    cd ../build
    tar zxf ../downloads/pkg-config-0.29.tar.gz
    cd pkg-config-0.29
    ./configure --with-internal-glib --prefix=/usr/local LDFLAGS="-framework CoreFoundation -framework Carbon"
    make
    make install
    cd ../../
```

4. libffi 3.2.1
    ```
    cd downloads
    curl -OL ftp://sourceware.org/pub/libffi/libffi-3.2.1.tar.gz
    cd ../build
    tar zxfv ../downloads/libffi-3.2.1.tar.gz
    cd libffi-3.2.1
    ./configure --prefix=/usr/local CC=clang
    make -j4
    make install
    cd ../../
```

5. gettext 0.19.8
    ```
    cd downloads
    curl -OL http://ftp.gnu.org/pub/gnu/gettext/gettext-0.19.8.tar.xz
    cd ../build
    tar zxfv ../downloads/gettext-0.19.8.tar.xz
    cd gettext-0.19.8
    ./configure --prefix=/usr/local CC=clang
    make -j4
    make install
    cd ../../
```

6. pcre 8.39
    ```
    cd downloads
    curl -OL http://internode.dl.sourceforge.net/project/pcre/pcre/8.39/pcre-8.39.tar.gz
    cd ../build
    tar zxfv ../downloads/pcre-8.39.tar.gz
    cd pcre-8.39
    ./configure --prefix=/usr/local --enable-utf8 --enable-unicode-properties CC=clang
    make -j4
    make install
    cd ../../
```

7. glib 2.50.1
    ```
    cd downloads
    curl -OL http://gemmei.acc.umu.se/pub/GNOME/sources/glib/2.50/glib-2.50.1.tar.xz
    cd ../build
    tar zxfv ../downloads/glib-2.50.1.tar.xz
    cd glib-2.50.1
    ./configure --prefix=/usr/local CC=clang
    make -j4
    make install
    cd ../../
```

8. autoconf
    ```
    cd downloads
    curl -OL http://ftpmirror.gnu.org/autoconf/autoconf-2.69.tar.gz
    cd ../build
    tar xzf ../downloads/autoconf-2.69.tar.gz
    cd autoconf-2.69
    ./configure --prefix=/usr/local
    make
    make install
    cd ../..
```

9. automake
    ```
    cd downloads
    curl -OL http://ftpmirror.gnu.org/automake/automake-1.15.tar.gz
    cd ../build
    tar xzf ../downloads/automake-1.15.tar.gz
    cd automake-1.15
    ./configure --prefix=/usr/local
    make
    make install
    cd ../../
```

10. libpng
    ```
    cd downloads
    curl -OL ftp://ftp.simplesystems.org/pub/png/src/libpng16/libpng-1.6.28.tar.gz
    cd ../build
    tar zxfv ../downloads/libpng-1.6.28.tar.gz
    cd libpng-1.6.28
    ./configure --prefix=/usr/local
    make
    make install
    cd ../..
```

11. glew 1.13.0
    ```
    cd downloads
    curl -L https://sourceforge.net/projects/glew/files/glew/1.13.0/glew-1.13.0.tgz/download > glew-1.13.0.tgz
    cd ../build
    tar zxfv ../downloads/glew-1.13.0.tgz
    cd glew-1.13.0
    make GLEW_DEST=/usr/local -j4
    make GLEW_DEST=/usr/local install
    cd ../..
```

12. readline 6.3
    ```
    cd downloads
    curl -OL https://ftp.gnu.org/gnu/readline/readline-6.3.tar.gz
    cd ../build
    tar zxfv ../downloads/readline-6.3.tar.gz
    cd readline-6.3
    ./configure --prefix=/usr/local CC=clang
    make -j4
    make install
    cd ../../
```

13. libtool
    ```
   cd downloads
   curl -OL http://ftpmirror.gnu.org/libtool/libtool-2.4.6.tar.gz
   cd build
   tar zxfv ../downloads/libtool-2.4.6.tar.gz
   cd libtool-2.4.6
   ./configure --prefix=/usr/local CC=clang
   make -j4
   make install
   cd ../../
```

14. libmpeg 2-0.5.1
    ```
    cd downloads
    curl -OL http://libmpeg2.sourceforge.net/files/libmpeg2-0.5.1.tar.gz
    cd build
    tar zxfv ../downloads/libmpeg2-0.5.1.tar.gz
    cd libmpeg2-0.5.1
    ./configure --prefix=/usr/local
    make -j4
    make install
    cd ../../
```

14. fs-uae
    ```
    git clone https://github.com/alpine9000/fs-uae.git
    cd fs-uae
    cp readline.pc /usr/local/lib/pkgconfig
    ./bootstrap
    ./configure CC=cc CXX=c++ --with-readline --enable-debug-symbols
    make -j4
    cd ..
 ```
    
