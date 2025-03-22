# Rustdesk - ПО удаленный стол
1. **[RustDesk](https://rustdesk.com/)**
2. **[RustDesk - Remote Desktop Software](https://rustdesk.com/docs/en/quickstart/install/)**
3. **To create a desktop shortcut for RustDesk:**
* Создайть файл с расширением .desktop в ~/Desktop/rustdesk.desktop).
```sh 
touch ~/Desktop/rustdesk.desktop
```
* Открыть файл в текстовом редакторе и вставить следующий код:
```sh
echo "[Desktop Entry]
Name=RustDesk
Comment=Remote desktop software
Exec=/usr/bin/rustdesk
Icon=/usr/share/icons/hicolor/scalable/apps/rustdesk.svg
Terminal=false
Type=Application
Categories=Network;RemoteAccess;" > ~/Desktop/rustdesk.desktop
```
* Сделать файл исполняемым:
```sh
chmod +x ~/Desktop/rustdesk.desktop
```

4. **Note:**
* If the icon path is different on your system, you may need to adjust the "Icon=" line accordingly. Also, if your desktop folder is named differently (e.g., in a non-English locale), you'll need to adjust the path accordingly.