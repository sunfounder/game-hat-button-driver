# Installation Guide
## Install Retro-Pie
在[retropie官网](https://retropie.org.uk/download/)下载最新版本的镜像（根据你的树莓派，选择对应的版本），将镜像文件下载到电脑上，并解压得到.img文件。

**balenaEtcher** is a graphical SD card writing tool that works on Mac OS, Linux and Windows, and is the easiest option for most users. balenaEtcher also supports writing images directly from the zip file, without any unzipping required. To write your image with balenaEtcher:

Download [balenaEtcher](https://www.balena.io/etcher/) and install it.
Connect an SD card reader with the SD card inside.
Open balenaEtcher and select from your hard drive the Raspberry Pi .img or .zip file you wish to write to the SD card.
Select the SD card you wish to write your image to.
Review your selections and click 'Flash!' to begin writing data to the SD card.

打开SD卡的config.tex文件进行屏幕分辨率的配置，在文件的底部加入以下内容:
hdmi_cvt=800 480 60 6
hdmi_group=2
hdmi_mode=87
hdmi_drive=2

将SD卡和USB键盘接入到树莓派上，打开开关，启动树莓派，进入系统后按键盘的F4，进入终端。

## 安装按键驱动
树莓派进行联网，

下载源码：
```bash
git clone <网站>
```
安装：
```bash
sudo python3 install.py
```
安装完成后提示是否重启， 输入Y确认：
```bash
Installation finished, do you want to reboot? (y/N) Y
```
最后按照提示设置对应的游戏按键，即可正常玩游戏了

## 添加新游戏

准备好相应的游戏ROMs,在[retropie官网](https://retropie.org.uk/docs/Transferring-Roms/)查阅详细步骤






