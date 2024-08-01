# Siegfried userspace toolchain

needed for building siegfried userspace programs

## How to compile

### Binutils

1. Make a build directory and cd into it
2. do ``(binutils path)/configure --target=x86_64-siegfried --prefix=(installation folder here) --with-sysroot``
3. do ``make && make install``

### GCC

1. Make another build directory and cd into it
2. do ``(gcc path)/configure --enable-languages=c,c++ --target=x86_64-siegfried --prefix=(installation folder here) --with-sysroot``
3. do ``make all-gcc && make all-target-libgcc && make install-gcc && make install-target-libgcc``
