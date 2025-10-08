[zh_CN](./README_ZH.md)
# Interaction
- This program is an interactive runner that allows you to quickly run Java, C++, PHP, JavaScript, and Python.
# install
- Use `dpkg-deb build` to package it into a DEB file.
```bash
dpkg-deb build Interaction
```
- If you are using Termux, we cannot install this DEB package with `dpkg -i` — this is because Android does not allow the installation of system packages. Therefore, we use the "moving files" method for installation.

1.unzip
  
```bash
dpkg -x Interaction.deb extracted/
```

2.moving

```bash
cp extracted/usr/local/bin/interaction $PREFIX/bin/
```

3.Grant executable permissions

```bash
chmod +x $PREFIX/bin/interaction
```

- After completing the above operations, you can use 'interaction' to run the program.
- Currently, there are ready-to-use DEB packages available in the Release description for you to download directly.
## use
- You can execute the program using the `interaction` command after installing it.
- After running the program, you will be prompted to enter "y" or "n":
 
- "n" means to exit;

- "y" means to start and download dependencies.
 
- Once the download is complete, you can enter the Java filename to run the Java program quickly.
- If you have already downloaded the dependencies, this prompt will not appear.
- Enter "cpp", "php", "js", or "python" to enter the corresponding running mode. The operation is consistent with the Java mode, and you can return to the Java mode using the "quit" command.
- You can exit the program via "quit".
