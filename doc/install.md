# Installation Guide
## Install Retro-Pie
在[retropie官网](https://retropie.org.uk/download/)下载最新版本的镜像（根据你的树莓派，选择对应的版本），将镜像文件下载到电脑上，并解压得到.img文件。

**balenaEtcher** is a graphical SD card writing tool that works on Mac OS, Linux and Windows, and is the easiest option for most users. balenaEtcher also supports writing images directly from the zip file, without any unzipping required. To write your image with balenaEtcher:

Download [balenaEtcher](https://www.balena.io/etcher/) and install it.
Connect an SD card reader with the SD card inside.
Open balenaEtcher and select from your hard drive the Raspberry Pi .img or .zip file you wish to write to the SD card.
Select the SD card you wish to write your image to.
Review your selections and click 'Flash!' to begin writing data to the SD card.

将SD卡和USB键盘接入到树莓派上，打开开关，启动树莓派，进入系统后按键盘的F4，进入终端。

## Pi4
目前Retro Pie 官方镜像 暂不支持Pi4， 需要手动安装测试版：
### 安装树莓派镜像
Install the latest version of Raspbian Buster on your Pi 4, if you haven’t already done so and boot into it. We recommend installing the lite version, which doesn't come with X Windows preloaded.
[Download](https://www.raspberrypi.org/downloads/raspbian/)
### 安装依赖:
```bash
    sudo apt-get update
    sudo apt-get dist-upgrade
    sudo apt-get install git
```

### 克隆`RetroPie-Setup`的Pi4测试版分支`fkms_rpi4`
```bash
    git clone -b fkms_rpi4 --depth=1 https://github.com/RetroPie/RetroPie-Setup
```

### 安装
```bash
    cd RetroPie-Setup
    sudo ./retropie_setup.sh
```

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

准备好相应的游戏ROMs，这里推荐一个非常酷的网站：http://coolrom.com/，你可以通过PC机，在里面下载各种游戏ROMs，点击Alternative download link进行下载

在[retropie官网](https://retropie.org.uk/docs/Transferring-Roms/)查阅详细步骤






