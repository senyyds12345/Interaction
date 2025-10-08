[zh_CN](./README_ZH.md)
# Interaction

这是一个交互式运行器，可以快速运行 Java、C++、PHP、 JavaScript 和 Python 程序。

## 安装方法

- 使用 `dpkg-deb build` 将其打包为 DEB 文件：
```bash
dpkg-deb build Interaction
```

- 如果您在使用 Termux，无法通过 dpkg -i 安装此 DEB 包，请使用"移动文件"方法进行安装：

1. 解压

```bash
dpkg -x Interaction.deb extracted/
```

1. 移动文件

```bash
cp extracted/usr/local/bin/interaction $PREFIX/bin/
```

1. 授予执行权限

```bash
chmod +x $PREFIX/bin/interaction
```

- 完成上述操作后，就可以使用 interaction 命令来运行程序了。
- 目前 Release 描述中提供了现成的 DEB 包，可供直接下载。

使用方法

- 安装后可以使用 interaction 命令执行程序。
- 运行程序后，会提示输入 "y" 或 "n"：
  - "n" 表示退出；
  - "y" 表示启动并下载依赖。
- 下载完成后，可以输入 Java 文件名来快速运行 Java 程序。
- 输入 "cpp"、"php"、"js" 或 "python" 可进入相应的运行模式。操作与 Java 模式一致，可以使用 "quit" 命令返回 Java 模式。
- 可以通过 "quit" 退出程序。