1. gcc-6.2.0 for OSX
    ```
    # svn checkout svn://gcc.gnu.org/svn/gcc/tags/gcc_6_2_0_release gcc-6.1.0-src
    # cd gcc-6.2.0-src
    # ./contrib/download_prerequisites
    # cd ..
    # mkdir gcc-6.2.0-build
    # cd gcc-6.2.0-build
    # ../gcc-6.2.0-src/configure --prefix=/usr/local --enable-languages=c,c++
    # make -j4
    # make install
```

2. SDL 2.0.5
    ```
    # curl -OL https://www.libsdl.org/release/SDL2-2.0.5.tar.gz
    # tar zxfv SDL2-2.0.5.tar.gz
    # cd SDL2-2.0.5
    # ./configure --prefix=/usr/local CC=clang
    # make -j4
    # make install
```

3. pkg-config
    ```
    # curl -OL https://pkg-config.freedesktop.org/releases/pkg-config-0.29.tar.gz
    # tar zxf pkg-config-0.29.tar.gz
    # cd pkg-config-0.29
    # ./configure --with-internal-glib --prefix=/usr/local LDFLAGS="-framework CoreFoundation -framework Carbon" CC=clang
    # make
    # make install
```

4. libffi 3.2.1
    ```
    # curl -OL ftp://sourceware.org/pub/libffi/libffi-3.2.1.tar.gz
    # tar zxfv libffi-3.2.1.tar.gz
    # cd libffi-3.2.1
    # ./configure --prefix=/usr/local CC=clang
    # make -j4
    # make install
```

5. gettext 0.19.8
    ```
    # curl -OL http://ftp.gnu.org/pub/gnu/gettext/gettext-0.19.8.tar.xz
    # tar zxfv gettext-0.19.8.tar.xz
    # cd gettext-0.19.8
    # ./configure --prefix=/usr/local CC=clang
    # make -j4
    # make install
```

6. pcre 8.39
    ```
    # curl -OL http://internode.dl.sourceforge.net/project/pcre/pcre/8.39/pcre-8.39.tar.gz
    # tar zxfv pcre-8.39.tar.gz
    # cd pcre-8.39
    # ./configure --prefix=/usr/local --enable-utf8 --enable-unicode-properties CC=clang
    # make -J4
    # make install
```

7. glib 2.50.1
    ```
    # curl -OL http://gemmei.acc.umu.se/pub/GNOME/sources/glib/2.50/glib-2.50.1.tar.xz
    # tar zxfv glib-2.50.1.tar.xz
    # cd glib-2.50.1
    # ./configure --prefix=/usr/local CC=clang
    # make -j4
    # make install
```

8. autoconf
    ```
    # curl -OL http://ftpmirror.gnu.org/autoconf/autoconf-2.69.tar.gz
    # tar xzf autoconf-2.69.tar.gz
    # cd autoconf-2.69
    # ./configure --prefix=/usr/local CC=clang
    # make
    # make install
```

9. automake
    ```
    # curl -OL http://ftpmirror.gnu.org/automake/automake-1.15.tar.gz
    # tar xzf automake-1.15.tar.gz
    # cd automake-1.15
    # ./configure --prefix=/usr/local CC=clang
    # make
    # make install
```

10. libpng
    ```
     # curl -OL ftp://ftp.simplesystems.org/pub/png/src/libpng16/libpng-1.6.25.tar.gz
     # tar zxfv libpng-1.6.25.tar.gz
     # cd libpng-1.6.25
     # ./configure --prefix=/usr/local CC=clang
     # make
     # make install
```

11. glew 1.13.0
    ```
    # curl -L https://sourceforge.net/projects/glew/files/glew/1.13.0/glew-1.13.0.tgz/download > glew-1.13.0.tgz
    # tar zxfv glew-1.13.0.tgz
    # cd glew-1.13.0
    # make GLEW_DEST=/usr/local -j4
    # make GLEW_DEST=/usr/local install
```

12. readline 6.3
    ```
    # curl -OL https://ftp.gnu.org/gnu/readline/readline-6.3.tar.gz
    # tar zxfv readline-6.3.tar.gz
    # cd readline-6.3
    # ./configure --prefix=/usr/local CC=clang
    # make -j4
    # make install
```

13. libtool
    ```
   # curl -OL http://ftpmirror.gnu.org/libtool/libtool-2.4.6.tar.gz
   # tar zxfv libtool-2.4.6.tar.gz
   # cd libtool-2.4.6
   # ./configure --prefix=/usr/local CC=clang
   # make
   # make install
```

14. libmpeg 2-0.5.1
    ```
    # curl -OL http://libmpeg2.sourceforge.net/files/libmpeg2-0.5.1.tar.gz
    # tar zxfv libmpeg2-0.5.1.tar.gz
    # cd libmpeg2-0.5.1
    # ./configure --prefix=/usr/local
    # make -j4
```

14. fs-uae
    ```
    # git clone https://github.com/alpine9000/fs-uae.git
    # cd fs-uae
    # cp readline.pc /usr/local/lib/pkgconfig
    # ./bootstrap
    # ./configure CC=cc CXX=c++ --with-readline --enable-debug-symbols
 ```
    
