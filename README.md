# LLVM-configuration

自用的，基于Ubuntu、LLVM配合clang前端、ninja编译的编译配置

Linux 需要安装 `cmake` `LLVM` `Clang` `Ninja-build`

VSCode 安装 `CMake` `CMake Tool` `Clangd` `codeLLDB` 插件

设置 `CMake Tool` 插件generator默认为 `Ninja`（在`Cmake: Edit CMake Cache(UI) `里）

编译步骤：
- 编写CMakeLists.txt
- 运行命令 `CMake: Scan for kits`，设置你想要的编译器，如`Clang\GCC`
- 运行命令 `CMake: Configure`，会将cmakelists的信息编译为makefile
- 运行命令 `Cmake:Build`，会按照Makefile将最终文件编译出来
- 点击下面的运行键（看着像播放键的按钮），运行最终文件

在项目根目录创建软链接：

```shell
ln -s ~/your project dir/build/compile_commands.json ~/your project dir
```
