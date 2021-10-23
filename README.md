# WARNING
**This repository is deprecated.**

**Development has been taken over by: https://github.com/matinlotfali/KDE-Rounded-Corners**
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>



# KDE-Rounded-Corners

This is a fork of https://sourceforge.net/projects/shapecorners/

When you disable window borders in System Settings --> Application Style --> Window Decorations --> Border size: No Borders you get sharp bottom window corners.

This effect rounds the corners of your windows.


![After](https://raw.githubusercontent.com/alex47/KDE-Rounded-Corners/master/screenshots/after.PNG)

# Dependencies:
Debian based (Ubuntu, Kubuntu, KDE Neon):
```
sudo apt install git cmake g++ gettext extra-cmake-modules qttools5-dev libqt5x11extras5-dev libkf5configwidgets-dev libkf5crash-dev libkf5globalaccel-dev libkf5kio-dev libkf5notifications-dev kinit-dev kwin-dev 
```
Fedora based
```
sudo dnf install git cmake gcc-c++ extra-cmake-modules qt5-qttools-devel qt5-qttools-static qt5-qtx11extras-devel kf5-kconfigwidgets-devel kf5-kcrash-devel kf5-kguiaddons-devel kf5-kglobalaccel-devel kf5-kio-devel kf5-ki18n-devel kf5-knotifications-devel kf5-kinit-devel kwin-devel qt5-qtbase-devel libepoxy-devel
```
OpenSUSE based
```
sudo zypper install git cmake gcc-c++ extra-cmake-modules libqt5-qttools-devel libqt5-qtx11extras-devel kconfigwidgets-devel kcrash-devel kguiaddons-devel kglobalaccel-devel kio-devel ki18n-devel knotifications-devel kinit-devel kwin5-devel libQt5Gui-devel libQt5OpenGL-devel libepoxy-devel
```

Arch based
```
sudo pacman -S git cmake extra-cmake-modules base-devel
yay -S qt5-tools
```

# How to build:
```
git clone https://github.com/alex47/KDE-Rounded-Corners

cd KDE-Rounded-Corners; mkdir qt5build; cd qt5build; cmake ../ -DCMAKE_INSTALL_PREFIX=/usr -DQT5BUILD=ON && make && sudo make install && (kwin_x11 --replace &)
```


It should be now activated.

For better results turn off the border size in:

System Settings --> Application Style --> Window Decoration
