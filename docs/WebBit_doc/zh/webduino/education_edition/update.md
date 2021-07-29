# 更新开发板固件

想要使用编辑器软件控制 Web:bit 开发板，需要为开发板 安装 或 更新 固件，可以选择下述多种方法给 开发板更新固件 或 恢复出厂设置 。

> 什么是编辑器？点此查看 [Web:bit 教育版 > 编辑器介绍](software.html#-1) 。

## 更新固件方法 1：使用 安装版 进行更新

> 什么是安装版？点此查看 [Web:bit 教育版 > 编辑器介绍 > 安装版](software.html#-5) 。

将开发板通过 Micro USB 线连接电脑，最上方会出现安装版的「版本号」（如：V1.2.4）以及「扫描 USB 设备」的提示，此时可以将开发板通过 USB 线连接电脑，让软件进行自动扫描并连接。

![](../../assets/webduino/education_edition/update/upload_3f793de122644f3c4fb1f17de0bcc634.png)

连接到开发板后，*安装版上方会出现开发板的 Device ID 以及固件版本号*，接着开启菜单栏（没有可以按下键盘的 *`Ctrl + W`* 出现），用鼠标选择「*工具> 设置 Web:bit WiFi*」，开始进行初始化设置。

![](../../assets/webduino/education_edition/update/upload_832cf2a13eb24e1c994fac3ea4d81373.png)

在电脑中打开 **安装版** 软件，将开发板通过 Micro USB 线连接电脑，确认安装版已经正确连接到开发板之后( 上方会出现开发板的 Device ID 以及版本号码)，按下`Ctrl + W` 打开工具栏，鼠标选择「*工具> 更新固件*」，就可以开始更新固件。

![](../../assets/webduino/education_edition/update/upload_bbb1222a27c9694ab3b8a1a71515c837.png)

如果检测到有新版本固件可供更新，也会在开发板连接电脑后弹出对话框提示。

![](../../assets/webduino/education_edition/update/upload_46c7a296ad1a32710e18c8dfb11a2ceb.png)

如果没有弹出对话框提示，也会在上方的信息文字里，出现提示更新的消息。

![](../../assets/webduino/education_edition/update/upload_986d0f00a17dbae92eff4feb19c21ab2.png)

点选更新后，会再度提示请勿关闭程序或移除 USB 线，按下确认后就开始更新。

![](../../assets/webduino/education_edition/update/upload_ffc83447d7c649a0c51d19fe6b930632.png)

更新时最上方的信息文字，会同步显示更新的进度。

![](../../assets/webduino/education_edition/update/upload_d83789034c2b05d079e1d6a6b03477f1.png)

更新直到 100% 之后会显示目前的版本号码，表示 开发板固件已经更新完成，如果没有反应请检查线材。

![](../../assets/webduino/education_edition/update/upload_e994b6436ddb867b584438e86d7b29b4.png)

## 恢复出厂固件

如果一直是「扫描 USB 设备」（长达三分钟），没有出现连接成功的消息，则表示 Web:Bit 开发板的固件可能有问题，此时可以用鼠标选择「工具 > 恢复出厂固件」进行固件修复。

![](../../assets/webduino/education_edition/update/upload_c50c3839f4d1fe1f8e60694b1c2813fb.png)

连接成功的可忽略此步骤，恢复出厂固件可能会让 Device ID 不同，请特别注意！

![](../../assets/webduino/education_edition/update/upload_c2ec7e8b5a7f87de903f5edf882fe41d.png)

## 更新固件方法 2：通过 Wi-Fi 远程更新

> 开发板联网需要先进行初始化，请查阅 [Web:bit 教育版 > 开发板设置](setup.md) 。

远程更新 ( OTA ) 可以在开发板连上网络后，连接远程服务器更新获取最新版本固件，更新步骤如下：

- 步骤 1、确认开发板已经可以正常连上 WiFi，若不行，请检查 WiFi 连接或重新进行初始化设定。
- 步骤 2、断开开发板电源。
- 步骤 3、连接开发板电源，**在显示白色跑马灯文字的时候，开始持续按住按钮A，直到开发板闪完红灯后没有亮绿灯表示失败，回到步骤 2 、直到出现绿灯熄灭后，此时会再听到蜂鸣器发出轻微的一个声响，此时放开按钮 A **。

![](../../assets/webduino/education_edition/update/ota-06.gif)

- 步骤 4、完成后会看到开发板的LED面板，由第一颗灯开始亮蓝灯，表示开始进行更新，*当蓝灯全部亮起接着熄灭后，表示更新完成*。

![](../../assets/webduino/education_edition/update/ota-07.gif)

- 步骤5、更新完成后开发板会闪红灯自动进行连接，连接成功会亮绿灯，接着绿灯熄灭，表示 OTA 更新固件完成。

## 恢复出厂设置

遇到奇怪的问题的时候无法解决，不妨试试还原硬件出厂时的设置，步骤如下：

- 步骤 1、断开开发板电源。
- 步骤 2、**同时按住按钮 A 和 B** 。
- 步骤 3、连接开发板电源，**听到蜂鸣器发出声响后放开按钮 A 与 B**，此时开发板已经恢复出厂设置。 ( **恢复设定值会将自定义 XXX 的 Wi-Fi 帐号、密码、自定义的 Device SSID 和密码清除，这个步骤会造成开发板无法连接所在场所的 Wi-Fi** )
- 步骤 4、重新进行初始化设定，请参考：[Web:bit 教育版 > 开发板设置](setup.md) 。
