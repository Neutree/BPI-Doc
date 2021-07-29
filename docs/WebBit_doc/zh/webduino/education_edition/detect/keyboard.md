# 键盘行为

鼠标和键盘是电脑必备的两大输入装置，熟悉了键盘的输入方式，就可以使用键盘进行简单交互，无论是要做成钢琴键盘还是游戏控制器都轻而易举，同时也可以搭配文字的输入，做出许多意想不到的互动效果。

## 检测键盘行为

「检测键盘行为」积木可以检测电脑键盘上大多数按键的按下与放开。

> 检测键盘行为积木*处于随时检测*的状态，*不需要搭配无限循环*。

![](../../../assets/webduino/education_edition/detect/keyboard/upload_cab0d8638477e4439b9bf927c1b71ace.jpg)

用过按下和放开两种行为，就可以在按下键盘的同时，让小怪兽说出对应按键名称，放开键盘后就不说话。

![](../../../assets/webduino/education_edition/detect/keyboard/upload_f2b9f50319a3b47a1adff6cafdc0dc7a.gif)

按下键盘的行为会「*连续执行指令*」，类似在打字的时候，如果按着某个按键不放，画面中就会出现一连串这个按键的文字，例如下图，设定按下键盘A 的时候小怪兽会往左旋转，执行后，持续按住A 怪兽就会持续旋转，放开A 怪兽就会停止，不需要设定放开的指令。

![](../../../assets/webduino/education_edition/detect/keyboard/upload_ab29dcdc4cf79cb980a9bac21baf2d2a.gif)

## 键盘控制小怪兽移动

积木可以*同时检测多个键盘控制行为*，通过键盘行为就能很简单的做出「按下上下左右键，小怪兽就会上下左右移动」。

![](../../../assets/webduino/education_edition/detect/keyboard/upload_307f1e13b196d6398223719f42edd2e3.gif)
