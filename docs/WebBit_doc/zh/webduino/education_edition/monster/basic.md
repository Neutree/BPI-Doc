# 小怪兽基本操作

编辑器设计了四只可爱的小怪兽，通过程序积木编排逻辑顺序，就能控制每只小怪兽的说话、声音、互动和行为等动作，甚至能进一步与实体开发板互动，做出更多好玩的有趣应用。

## 小怪兽积木清单 ( 基本操作 )

基本操作小怪兽的积木分别有讲话、展示图片、情绪、改变位置、改变角度、改变大小、显示隐藏和阶层...等，可以通过这些积木控制小怪兽的外在表现。

![](../../../assets/webduino/education_edition/monster/basic/upload_ecaf893841c42dfab8dba2e59219b3f0.png)

## 讲话＆不讲话

「讲话」和「不讲话」积木可以让小怪兽讲出指定的文字，或不要讲出文字，通过下拉选单也可以选择哪一只小怪兽讲话，或所有小怪兽一起讲话。

![](../../../assets/webduino/education_edition/monster/basic/upload_2e3b52771cffb4aa57eba477b5c2a786.png)

只要在讲话的积木后方，连接指定的文字，执行后小怪兽就会说出指定的文字。

![](../../../assets/webduino/education_edition/monster/basic/upload_705418bdeba488d8a1aac5daf3ff86f5.png)

只要把文字留空，或者使用不说话的积木，就能够让小怪兽不说话。

![](../../../assets/webduino/education_edition/monster/basic/upload_e559ef990c771072f48b1693c8b762b9.png)

## 展示图片

「展示图片」积木可以让小怪兽展示一张「网络图片」。

![](../../../assets/webduino/education_edition/monster/basic/upload_b7edb18992b7d500b6902688a5b9e318.png)

举例来说，从百度百科上搜寻[蒙娜丽莎]，可以得到这张图片的「[网址](https://upload.wikimedia.org/wikipedia/commons/thumb/e/ec/Mona_Lisa%2C_by_Leonardo_da_Vinci%2C_from_C2RMF_retouched.jpg/460px-Mona_Lisa%2C_by_Leonardo_da_Vinci%2C_from_C2RMF_retouched.jpg#_blank)」，复制图片网址，贴到小怪兽展示图片的文字空格内，执行后，就会看见小怪兽展示这张图片。

> 目前图片格式仅支持 jpg、jpeg、png、gif（图片网址结尾必须带有图片格式才能显示图片）

![](../../../assets/webduino/education_edition/monster/basic/upload_0e42941e1908cd0eee54be33f33dc605.png)

## 情绪

「情绪」积木可以改变小怪兽的情绪，包含开心、惊讶、生气、难过和随机情绪。

![](../../../assets/webduino/education_edition/monster/basic/upload_590cfe6b6bb11b37e0785e45a28d3591.png)

选择对应的小怪兽 ( 也可以四只同时 )，选择对应的情绪，执行后就会看见小怪兽的情绪变化。

![](../../../assets/webduino/education_edition/monster/basic/upload_1ab6008309379d6e26ac09ad81d20011.png)

## 改变位置

「改变位置」积木可以指定小怪兽改变*目前的位置*，选项有往上、往下、往左、往右、随机或朝向鼠标方向。

![](../../../assets/webduino/education_edition/monster/basic/upload_64c0e2ae93164965ef2800de7c4d081f.png)

如下图，搭配「循环十次」和「等待 0.1 秒」积木，就能够让小怪兽往右上方移动。

![](../../../assets/webduino/education_edition/monster/basic/basic-10.gif)

如果使用「无限循环」积木，搭配「朝着鼠标位置」的设定，就能够让小怪兽追着鼠标移动。

![](../../../assets/webduino/education_edition/monster/basic/basic-11.gif)

## 定位

「定位」积木能够把小怪兽摆放到指定的坐标位置。

![](../../../assets/webduino/education_edition/monster/basic/basic-12.png)

怪兽的座标系统采用*笛卡尔直角座标系统* (直角座标系统)，往上y 为正，往右x 为正，而(0,0) *原点位在怪兽互动舞台的左下角*，指定小怪兽xy 坐标，执行后小怪兽就会出现在指定的位置。

![](../../../assets/webduino/education_edition/monster/basic/basic-13.jpg)

## 旋转角度

「旋转角度」可以指定小怪兽改变*目前的角度*，选项有往左或往右。

![](../../../assets/webduino/education_edition/monster/basic/basic-14.png)

搭配「无限循环」积木，就能让小怪兽不断的每隔 0.1 秒旋转 10 度。

![](../../../assets/webduino/education_edition/monster/basic/basic-15.gif)

## 面朝方向

「面朝方向」角度可以指定小怪兽旋转的角度，顺时针为正，逆时针为负。

![](../../../assets/webduino/education_edition/monster/basic/basic-16.png)

因为「面朝方向」是指定一个角度，如果要做到和前一个积木「旋转角度」一样的效果，可以使用变量搭配「无限循环」积木，在每一次执行时修改变量数值即可。

![](../../../assets/webduino/education_edition/monster/basic/basic-17.gif)

## 自动面朝鼠标方向

「自动面朝鼠标方向」积木能让小怪兽转到鼠标所在的方向，有自动和停止两个选项。

![](../../../assets/webduino/education_edition/monster/basic/basic-18.png)

因为「自动面朝鼠标方向」只会执行一次，所以如果要让小怪兽不断的面向鼠标，就必须搭配无限循环的积木，如下图，执行后小怪兽就会自动面向鼠标旋转。

![](../../../assets/webduino/education_edition/monster/basic/basic-19.gif)

## 取得座标和角度

「取得座标和角度」积木能够读取小怪兽当前的 X 座标、Y 座标和旋转角度。

![](../../../assets/webduino/education_edition/monster/basic/basic-20.png)

下图的例子，就能让小怪兽自己讲出自己的 X 座标、Y 座标和旋转角度。

![](../../../assets/webduino/education_edition/monster/basic/basic-21.jpg)

## 尺寸放大缩小

「尺寸放大缩小」积木可以指定小怪兽改变*目前的大小*，选项有放大或缩小。

![](../../../assets/webduino/education_edition/monster/basic/basic-22.png)

搭配「循环十次」和「等待 0.1 秒」积木，执行后，就能够让小怪兽逐渐变大。

![](../../../assets/webduino/education_edition/monster/basic/basic-23.gif)

## 尺寸百分比

「尺寸百分比」积木可以指定小怪兽放大缩小的百分比。

![](../../../assets/webduino/education_edition/monster/basic/basic-24.png)

由于 100% 表示原本怪兽大小，所以 200% 就会是一倍大，50% 则是会缩成 1/2 大小，下图通过尺寸百分比，分别让四只小怪兽呈现不同尺寸大小。

![](../../../assets/webduino/education_edition/monster/basic/basic-25.jpg)

## 显示/不显示

「显示/不显示」积木可以指定小怪兽是否显示在互动舞台区。

![](../../../assets/webduino/education_edition/monster/basic/basic-26.jpg)

## 阶层

「阶层」积木可以指定小怪兽排列的阶层，最上层在最前面，最下层在最后面。

![](../../../assets/webduino/education_edition/monster/basic/basic-28.png)

通过「循环」以及「等待」积木，能够让小怪兽的阶层依序显示在最前面。

![](../../../assets/webduino/education_edition/monster/basic/basic-29.gif)

## 回到原始状态

「回到原始状态」积木可以让小怪兽回到初始状态，初始状态包含不说话、预设座标、预设旋转角度和预设尺寸大小。

![](../../../assets/webduino/education_edition/monster/basic/basic-27.png)
