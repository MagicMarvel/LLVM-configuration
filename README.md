# LLVM-configuration

自用的，基于Ubuntu、LLVM配合clang前端、ninja编译的编译配置

Linux 需要安装 `cmake` `LLVM` `Clang` `Ninja-build`

VSCode 安装 `CMake` `CMake Tool` `Clangd` `codeLLDB` 插件

设置 `CMake Tool` 插件generator默认为 `Ninja`

在项目根目录创建软链接：

```shell
ln -s ~/your project dir/build/compile_commands.json ~/your project dir
```
