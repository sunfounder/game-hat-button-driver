## 驱动安装
1.在retropie官网下载最新版本的镜像（根据你的树莓派，选择对应的版本），将镜像文件下载到电脑上，并解压得到.img文件。
2.将SD卡连接到电脑，打开Win32DiskImager.exe软件，选择第1步准备的.img文件，点击write烧写镜像。
3.将SD卡和USB键盘接入到树莓派上，打开Battery，启动树莓派，进入系统后按键盘的F4，进入终端。
4.树莓派进行联网，执行git clone <网站>下载游戏机驱动所需文件gpio-joystick,gpio-joystick.py,install.py
5.在树莓派上执行sudo python3 install.py以安装游戏驱动
6.最后设置对应的游戏按键，即可正常玩游戏了

## 添加新游戏
1.由于大部分游戏容量很大，在添加游戏前，我们先进行文件系统扩展。在配置界面选择RASPI-CONFIG，回车
选择7 Advanced Options -> A1 Expand Filesystem，回车-》Finish。(这个过程需要接上USB键盘进行操作)
选择Ok，对系统进行重启。重启后，文件系统扩展完成。
2.准备好相应的游戏ROMs，这里推荐一个非常酷的网站：http://coolrom.com/，你可以通过PC机，在里面下载各种游戏ROMs，点击Alternative download link进行下载
3.将解压到的文件传输到树莓派上/home/pi/RetroPie/roms相对应的ROMS文件夹中。
4.之后在模拟器选择界面，按"Start"->QUIT->RESTART EMULATIONSTATION，按"A"确定。重启模拟器之后即可看到新加入的游戏。






