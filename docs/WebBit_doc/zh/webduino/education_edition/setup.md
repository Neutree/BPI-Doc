# 开发板设置

在往下使用开发板的 WIFI 联网功能之前，需要先进行初始化设置，通过本节的初始化设置可以让开发板可以连上网络（Internet），还可以够自定义开发板的 WIFI 显示名称和密码，更是可以通过网络进行远程更新（OTA）。

> 初始化后可以**通过「Wi-Fi」控制开发板**，如果只是使用「USB 控制」开发板，则可以跳过初始化设置。

## 初始化方法 1：使用安装版进行初始化

> 什么是安装版？点此查看 [Web:bit 教育版 > 编辑器介绍 > 安装版](software.html#-5) 。

使用安装版按照下列步骤进行初始化设置。

### 步骤 1、进入菜单 > 工具 > 设置 Web:bit WIFI

将开发板通过 Micro USB 线连接电脑，打开安装版后，软件顶栏会出现安装版的「版本号（如：V1.2.4）」以及「扫描 USB 设备」的提示（如下图），此时可以将开发板通过 USB 线连接电脑，让软件进行自动扫描并连接开发板。

![](../../assets/webduino/education_edition/setup/upload_3f793de122644f3c4fb1f17de0bcc634.png)

连接到开发板后，*软件顶栏会出现开发板的 Device ID 以及固件版本号*（如下图），接着查看菜单栏（没有看到需要按下键盘的*`Ctrl + W`* 开启），用鼠标选择「*工具> 设置 Web:bit WiFi*」，开始进行初始化设置。

![](../../assets/webduino/education_edition/setup/upload_c792e42e263f5a843da6255867d1a77f.png)

> *注意！没有出现如图连接情况，请使用 [Web:bit 教育版 > 更新开发板固件 > 恢复出厂固件](update.html#-2)。

### 步骤 2、设置 Web:bit Wi-Fi 的名称（SSID）与密码

点击设置 WiFi 后，会弹出一个对话窗，此时要填入想要连接的 WiFi 的名称和密码。 ( 这里就填入自己所在场所(例如：公司、学校或家里）的 Wi-Fi 帐号和密码 )

设置 WIFI 连接的名称（SSID），存在配置则会读回，默认值是 `webduino.io` 。

![](../../assets/webduino/education_edition/setup/upload_621ed89a98ab4e189626b6f46381ddd5.png)

设置 WIFI 连接的 密码 ，存在配置则会读回，默认值是 `webduino` 。

![](../../assets/webduino/education_edition/setup/upload_3e99dc9aeb3caa3e2793b1528718f1e0.png)

设置完成后，会弹出一个对话窗口，询问是否关闭 USB 连接，如果选择「确定」，开发板就会通过先前的 Wi-Fi 的帐号与密码，连接到指定的 Wi-Fi ，如果选择「取消」，就会关闭 Wi-Fi 连接功能，此时只能使用 USB 连接操作。

![](../../assets/webduino/education_edition/setup/upload_4b45f7eb17a57e6a31f1d483db93047e.png)

若选择关闭 USB 连接功能，开发板会进入 WIFI 连接模式。

此时开发板会重启并闪烁红灯，当 **红灯熄灭** 且 **绿灯亮起** 之后，表示 Web:Bit 开发板已经成功连接上 WiFi 。

![](../../assets/webduino/education_edition/setup/upload_9fc275139e019a3ba9f86d0fd133c762.gif)

- 若红灯持续闪烁或恒亮，请拔掉电源，重新操作步骤 1 与步骤 2 。

- 若红灯闪完后亮起「蓝灯」而不是绿灯，表示已有新版本可以进行下载更新，请参考[Web:bit 教育版 > 更新开发板固件](update.html#-1) 。

![](../../assets/webduino/education_edition/setup/upload_184a8ab60565dbd34c2e4cac4a0a530b.gif)

## 初始化方法 2：WIFI 连接到开发板进行初始化

如果想通过无线控制开发板，可以通过有 Wi-Fi 连接功能的笔记本电脑或移动设备（手机），连接到开发板的 WIFI 热点进行初始化设置，相关步骤如下所示：

### 步骤 1、接上电源，输入 WiFi 帐号和密码进行连接

使用 USB 线为开发板接上电源，此时开发板正面的 矩阵 LED 会滚动显示一串文字( *默认是 bit 三个英文 + 四个数字* )，如下图的滚动显示的 bit1234 。

![](../../assets/webduino/education_edition/setup/setup-05.gif)

这串文字会出现在其他可以连接 WIFI 的设备的 WiFi 名称列表中，例如下图显示的 bit1234 ，在 WiFi 搜索界面中就会看到 bit1234 的 WIFI 名称。

![](../../assets/webduino/education_edition/setup/setup-06.jpg)

滚动结束后，第一次使用开发板未进行初始化设置，就无法连上外网（Internet）服务器，所以 **会闪红灯，或者红灯恒亮** 。这时请准备一台具有 WiFi 功能的电脑、手提或移动设备（手机），使用这台设备进行 Wi-Fi 搜索，连接刚刚看到为「bitXXXX」的装置( 以上述的例子就是 bit1234 )，找到该设备后，输入默认密码 **12345678** ，进行连接即可。

### 步骤 2、设置 WiFi 帐号密码与显示名称

*确认连接成功*后，打开浏览器 ( 建议使用 Chrome )，地址栏输入 `192.168.4.1` 会进入到 Web:Bit 开发板的设置画面，画面中包含以下几种设置：

![](../../assets/webduino/education_edition/setup/upload_6e1c12f5120345e4e97d8d05d9251791.png)

> 可在下图表格中找到对应设置项详细解释。

![](../../assets/webduino/education_edition/setup/settings.png)

设置完成后按下 **SUBMIT** 保存，出现 **SAVE OK** 的字样表示设置成功。

![](../../assets/webduino/education_edition/setup/upload_3ec8cc6a377c2a2cd987be93d391da60.png)

此时开发板会重启并闪烁红灯，当 **红灯熄灭** 且 **绿灯亮起** 之后，表示 Web:Bit 开发板已经成功连接上 WiFi 。

![](../../assets/webduino/education_edition/setup/upload_9fc275139e019a3ba9f86d0fd133c762.gif)

- 若红灯持续闪烁或恒亮，请拔掉电源，重新操作步骤 1 与步骤 2 。

- 若红灯闪完后亮起「蓝灯」而不是绿灯，表示已有新版本可以进行下载更新，请参考[Web:bit 教育版 > 更新开发板固件](update.html#-1) 。

![](../../assets/webduino/education_edition/setup/upload_184a8ab60565dbd34c2e4cac4a0a530b.gif)
