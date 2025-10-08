# Interaction
- This program is an interactive runner that allows you to quickly run Java, C++, PHP, JavaScript, and Python.
# install
- Use  `dpkg-deb build`  to package it into a DEB file.
```dpkg-deb build Interaction```
- If you are using Termux, we cannot install this DEB package with  dpkg -i —this is because Android does not allow the installation of system packages. Therefore, we use the "moving files" method for installation.
- unzip
```dpkg -x Interaction.deb extracted/```
- moving
```cp extracted/usr/local/bin/interaction $PREFIX/bin/```
- Grant executable permissions
```chmod +x $PREFIX/bin/interaction```
- After completing the above operations, you can use  interaction  to run the program.
