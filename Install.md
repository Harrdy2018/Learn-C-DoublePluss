## Windows上安装C++
* 安装```MSYS2```
```txt
网址: https://www.msys2.org/

学习网址: http://events.jianshu.io/p/2a3ff0d4f53a

VSCODE: https://code.visualstudio.com/docs/cpp/config-mingw

MSYS2是一组工具和库，提供了一个易于使用的环境，用于构建、安装和运行原生的Windows软件。
```
* pacman
```sh
mysys2里使用了pacman来管理软件包。

-Msys2使用pacman管理软件。pacman的基本使用如下：

pacman -S <packge-name>     # 安装软件
pacman -U <gz-file>         # 安装本地包，其扩展名为 pkg.tar.gz
pacman -Syu                 # 同步Msys2源，并更新
pacman -Sy                  # 仅同步源
pacman -Su                  # 更新系统
pacman -Sy <packge-name>    # 同步源后再安装软件
pacman -R <packge-name>     # 该命令将只删除包，不包含该包的依赖。
pacman -Rs <packge-name>    # 在删除包的同时，也将删除其依赖。
pacman -Rd <packge-name>    # 在删除包时不检查依赖。
pacman -Ss <keywords>       # 这将搜索含关键字的包。
pacman -Qi <packge-name>    # 查看有关包的信息。
```
* 安装软件
```sh
pacman -S mingw-w64-x86_64-gcc
pacman -S mingw-w64-x86_64-make
pacman -S mingw-w64-x86_64-cmakepacman -S mingw-w64-x86_64-svn
pacman -S mingw-w64-x86_64-vim
pacman -S mingw-w64-x86_64-capstone
pacman -S mingw-w64-x86_64-glfw
pacman -S mingw-w64-x86_64-glm
pacman -S mingw-w64-x86_64-file
pacman -S mingw-w64-x86_64-llvm
pacman -S mingw-w64-x86_64-nlohmann-json
pacman -S mingw-w64-x86_64-openssl
```
* Cmake安装
```sh
查询cmake软件
$ pacman -Sl | grep cmake

clangarm64 mingw-w64-clang-aarch64-cmake 3.25.2-1
clangarm64 mingw-w64-clang-aarch64-extra-cmake-modules 5.103.0-1
clangarm64 mingw-w64-clang-aarch64-python-sphinxcontrib-moderncmakedomain 3.25.0-1
mingw32 mingw-w64-i686-cmake 3.25.2-1
mingw32 mingw-w64-i686-cmake-doc-qt 3.25.2-1
mingw32 mingw-w64-i686-cmakerc 2.0.1-1
mingw32 mingw-w64-i686-extra-cmake-modules 5.103.0-1
mingw32 mingw-w64-i686-python-sphinxcontrib-moderncmakedomain 3.25.0-1
mingw64 mingw-w64-x86_64-cmake 3.25.2-1
mingw64 mingw-w64-x86_64-cmake-doc-qt 3.25.2-1
mingw64 mingw-w64-x86_64-cmakerc 2.0.1-1
mingw64 mingw-w64-x86_64-extra-cmake-modules 5.103.0-1
mingw64 mingw-w64-x86_64-python-sphinxcontrib-moderncmakedomain 3.25.0-1
ucrt64 mingw-w64-ucrt-x86_64-cmake 3.25.2-1
ucrt64 mingw-w64-ucrt-x86_64-cmake-doc-qt 3.25.2-1
ucrt64 mingw-w64-ucrt-x86_64-cmakerc 2.0.1-1
ucrt64 mingw-w64-ucrt-x86_64-extra-cmake-modules 5.103.0-1
ucrt64 mingw-w64-ucrt-x86_64-python-sphinxcontrib-moderncmakedomain 3.25.0-1
clang32 mingw-w64-clang-i686-cmake 3.25.2-1
clang32 mingw-w64-clang-i686-cmake-doc-qt 3.25.2-1
clang32 mingw-w64-clang-i686-cmakerc 2.0.1-1
clang32 mingw-w64-clang-i686-extra-cmake-modules 5.103.0-1
clang32 mingw-w64-clang-i686-python-sphinxcontrib-moderncmakedomain 3.25.0-1
clang64 mingw-w64-clang-x86_64-cmake 3.25.2-1
clang64 mingw-w64-clang-x86_64-cmake-doc-qt 3.25.2-1
clang64 mingw-w64-clang-x86_64-cmakerc 2.0.1-1
clang64 mingw-w64-clang-x86_64-extra-cmake-modules 5.103.0-1
clang64 mingw-w64-clang-x86_64-python-sphinxcontrib-moderncmakedomain 3.25.0-1
msys cmake 3.25.1-1
msys cmake-emacs 3.25.1-1
msys cmake-vim 3.25.1-1
msys icmake 9.03.01-1


安装cmake软件
$ pacman -S mingw-w64-x86_64-cmake
```
* make软件
```sh
pacman -Sl | grep make

mingw64 mingw-w64-x86_64-bmake 20181221-8
mingw64 mingw-w64-x86_64-cmake 3.25.2-1 [installed]
mingw64 mingw-w64-x86_64-cmake-doc-qt 3.25.2-1
mingw64 mingw-w64-x86_64-cmakerc 2.0.1-1
mingw64 mingw-w64-x86_64-dmake 4.12.2.2-1
mingw64 mingw-w64-x86_64-extra-cmake-modules 5.103.0-1
mingw64 mingw-w64-x86_64-make 4.4-2 [installed]
mingw64 mingw-w64-x86_64-premake 5.0beta1-1
mingw64 mingw-w64-x86_64-python-sphinxcontrib-moderncmakedomain 3.25.0-1
mingw64 mingw-w64-x86_64-xmake 2.7.7-1
```
* git软件
```sh
pacman -Sl | grep git
```
