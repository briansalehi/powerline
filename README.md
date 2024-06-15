# Powerline

Set of power controlling gadgets for indoor use.

## CONTRIBUTION

Contribution of any kind is welcome to this project.

Required packages to work with this project is:

* `clang` or `g++`
* `make`
* `cmake`
* `libboost-dev`, `libboost-program-options`
* `libgtest-dev`
* kicard

Build project:

```sh
git clone https://github.com/briansalehi/powerline.git
cmake -S powerline -B powerline-build -D CMAKE_BUILD_TYPE=Release -D CMAKE_INSTALL_PREFIX=$HOME/.local
cmake --build powerline-build --parallel $(nproc) --target all
```

Permanent use:

```sh
cmake --install powerline-build
```

Run tests:

```sh
ctest --build-and-test powerline powerline-build
```
## LICENSE

This project is licensed under [MIT License](LICENSE.md).
