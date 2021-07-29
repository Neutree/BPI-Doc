# 小怪兽互动＆舞台

除了可以设定小怪兽的位置或大小，编辑器更能让我们与小怪兽互动，例如用鼠标点击小怪兽、小怪兽互相碰撞、碰撞舞台画面边缘...等。

## 小怪兽积木清单 ( 互动＆舞台 )

互动＆舞台的积木分别有鼠标点击小怪兽、鼠标触碰小怪兽、小怪兽互相碰撞、小怪兽碰撞舞台边缘、碰到舞台边缘就反弹、更换舞台背景和设定为全屏幕。

![](../../../assets/webduino/education_edition/monster/event/event-01.png)

## 鼠标点击

「鼠标点击」积木可以在鼠标点击小怪兽时，让小怪兽做指定的事情。

> 鼠标点击积木「*不需要放在循环内*」就可重复检测，并在后台执行。

![](../../../assets/webduino/education_edition/monster/event/upload_bd5d493660fdf95650cfd71875b09f68.png)

下图的例子，点击绿色小怪兽时会说话，点击红色小怪兽会放大，点击黄色小怪兽会旋转，点击蓝色小怪兽会改变情绪。

![](../../../assets/webduino/education_edition/monster/event/event-03.gif)

## 鼠标触碰

「鼠标触碰」积木包含两个行为动作，分别是鼠标触碰到小怪兽要做什么事，以及鼠标离开小怪兽后要做什么事。

> 注意，离开的行为动作一定会接在触碰之后，鼠标触碰积木「*不需要放在循环内*」就可重复检测。

![](../../../assets/webduino/education_edition/monster/event/upload_6eee2e14f316f79216ef294e531284c1.png)

下图的例子，在鼠标触碰到绿色小怪兽时，小怪兽的情绪会开心，鼠标离开后小怪兽又恢复正常的情绪。

![](../../../assets/webduino/education_edition/monster/event/upload_bd4c4a7f42b86231ee1d30f7da6d1681.gif)

## 互相触碰

「互相触碰」积木可以检测小怪兽彼此之间是否有触碰。

>「互相触碰」积木「*只会检测一次*」，必须*搭配循环*，才能重复检测。

![](../../../assets/webduino/education_edition/monster/event/upload_eab6bd21822786b42a47fe7afd4e3edc.png)

以下图为例，搭配「无限循环」积木就能不断检测小怪兽是否互相触碰。用鼠标拉动小怪兽，当两只小怪兽相碰时，小怪兽就变成惊讶的情绪，分开后又恢复正常。

![](../../../assets/webduino/education_edition/monster/event/event-07.gif)

## 触碰舞台边缘

「触碰舞台边缘」积木可以检测小怪兽是否触碰到互动舞台的四个边，或指定检测碰到上、下、左、右四个边的行为。

>「触碰舞台边缘」积木「*只会检测一次*」，必须*搭配循环*，才能重复检测。

![](../../../assets/webduino/education_edition/monster/event/upload_d046836899bee6928e3cb4e801b7c6a2.png)

以下图为例，搭配「无限循环」积木就能让小怪兽碰到舞台画面上边缘或下边缘时，变成开心的情绪，碰到左边缘或右边缘则呈现生气的情绪，没有碰到时则是正常情绪。

![](../../../assets/webduino/education_edition/monster/event/event-09.gif)

## 触碰舞台边缘就反弹

「触碰舞台边缘就反弹」积木是「触碰舞台边缘」积木的简化版，将碰触后的行为单一化为「反弹」，反弹表示位置的相反，*如果碰到舞台左右两侧，则小怪兽移动的X 方向会相反，如果碰到舞台上下两侧，则小怪兽移动的Y 方向会相反*。

>「触碰舞台边缘就反弹」积木「*只会检测一次*」，必须*搭配循环*，才能重复检测。

![](../../../assets/webduino/education_edition/monster/event/upload_9cc804bee48cd25db97ef0415aa5de8d.png)

以下图为例，搭配「无限循环」积木碰到舞台边缘时就会反弹。

![](../../../assets/webduino/education_edition/monster/event/upload_2054073407edffc93259cee64ea8d559.gif)

## 更换舞台背景颜色或图片

「更换舞台背景颜色」和「更换舞台背景图片」，可以改变怪兽舞台背景为指定的颜色或图片，图片只要填入图片网址，执行后就会更换。 ( 图片支持 jpg、jpeg、png 和 gif )

![](../../../assets/webduino/education_edition/monster/event/upload_a0ffebb197b6a1b7e624df95575db57e.png)

举例来说，找一张[清明上河图](https://theme.npm.edu.tw/opendata/att/collectionPic/04015934/17024347.jpg#_blank)的图片网址，将网址贴上在背景图片的文字积木内，执行后就会看见舞台背景变成清明上河图了。

![](../../../assets/webduino/education_edition/monster/event/upload_0a5192dcef98295928291f37dc3aa941.png)

## 设定舞台为全屏幕

「设定舞台为全屏幕」积木不影响任何操作，只会在「执行时」把怪兽互动舞台变成全屏幕大小。

![](../../../assets/webduino/education_edition/monster/event/upload_c7f81fc1821ae721f0a1ae538cf657d7.png)

如果不想使用该功能，也可以手动操作，点选怪兽互动舞台右上方的小按钮，也可以进行全屏幕的切换。

![](../../../assets/webduino/education_edition/monster/event/event-15.jpg)

## 取得舞台尺寸

「取得舞台尺寸」积木可以取得当下怪兽互动舞台的宽度或高度。

![](../../../assets/webduino/education_edition/monster/event/upload_3f0c3896ee92a0b281e3cb96344ac1f5.png)

下图的例子会在执行的时候，绿色小怪兽讲出舞台宽度，红色小怪兽讲出舞台高度。

![](../../../assets/webduino/education_edition/monster/event/upload_990e0968794979db21161874e12d667e.png)
