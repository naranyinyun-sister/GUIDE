# 概述

## 这应该写啥比较合适?

?> 需要验证码吗? MI8SE-Rubbishy AMOLED

这是一份Xiaomi 8 SE的刷机手册,其实也不是非要写这个,只是我在研究 docsify 想不出来写什么而已

> 本手册由Docsify强力驱动
> 
> 编纂/构建 : 纳兰音韵
> 
> SGSI-Rom Rransplant : 虾滑被吃掉了
> 
> 本项目由Cloudflare Pages托管,使用Cloudflare CDN加速(当然也可能是减速)

求求了,点一下[这个](https://nalanyinyun.ml/)和[这个](https://blog.nalanyinyun.ml/),最近访问量实在惨淡，~~客官，不来玩吗？~~  

**免责声明:您因本手册或刷写本手册提供的资源而造成意外事故时，我们不与您的问题有任何直接或间接关联**  
# 准备

## 硬件材料

一台**已解锁**的小米8SE

一台**已安装驱动**的电脑

一根**数据**线

一颗**能够正常使用**的脑子

## 软件材料

[小米8SE扩容工具](https://dl.xiahuabeichidiaole.ml/%E8%99%BE%E6%BB%91%E7%9A%84Electronic%20Product%E8%B5%84%E6%BA%90%E5%BA%93/%E8%99%BE%E6%BB%91%E5%AE%9A%E5%88%B6Android/MI%208%20SE/System%E6%89%A9%E5%AE%B9%EF%BC%885G%EF%BC%89.zip)

[MIUI13 For 8 SE](https://dl.xiahuabeichidiaole.ml/%E8%99%BE%E6%BB%91%E7%9A%84Electronic%20Product%E8%B5%84%E6%BA%90%E5%BA%93/%E8%99%BE%E6%BB%91%E5%AE%9A%E5%88%B6Android/MI%208%20SE/MIUI13%20For%20MI%208%20SE(Copper%20hot%20pot).zip)

[禁用AVB工具](https://dl.xiahuabeichidiaole.ml/%E8%99%BE%E6%BB%91%E7%9A%84Electronic%20Product%E8%B5%84%E6%BA%90%E5%BA%93/%E8%99%BE%E6%BB%91%E5%AE%9A%E5%88%B6Android/MI%208%20SE/%E5%B0%8F%E7%B1%B38se%20%20%E5%8D%A1fastboot%E4%B8%93%E7%94%A8.zip)

<details>
  <summary>常见问题</summary>

     Q:无法下载--A:使用电脑下载/使用Chrome或Edge/使用下载器
    
     Q:网站打不开--A:自备工具,服务器在阿美丽卡

</details>

## 知识准备

您必须了解了解以下概念

- Bootloader

- AVB

- Fastboot/Recovery

您必须了解一些基本的计算机名词,如果一窍不通并依旧打算继续,**您可以去附近的三甲医院挂脑科看看**

> **您可以去:天坛医院、宣武医院、解放军总医院、协和医院等顶级脑科医院就诊**

如果您有一定的英语基础,您可以更快的了解本手册,如果您没有,也没关系,善用[翻译工具](https://translate.google.cn)

# 快速开始

## 刷入第三方Recovey

重启您的8SE至Fastboot模式,刷入TWRP(推荐)

您可以使用其他方法,我们推荐使用ADB,配置环境可以[参考](https://blog.nalanyinyun.ml/p/adb-flash/)

连接手机(不要使用USB3.0)

打开终端,输入

```
fastboot recovery [path/firename]

adb reboot recovery
```

## System扩容

进入Recovery,使用MTP将解压后的"MI8SE_5GB_System.zip"传输到设备中

选择刷入,选择"MI8SE_5GB_System.zip",点击刷入并滑动确认

在清除中双清和格式化DATA(Dirty Flash可能支持,但推荐格式化)

**可能需要重启才能正确挂载DATA,请自行解决覆盖问题**

<details>
<summary>重要提示</summary>

你已经修改了System分区,在不关闭AVB的情况下无法启动设备,本次MIUI13自动关闭AVB

如果你需要回官方,请刷入"MI8SE_BACK.zip"或使用工具关闭AVB(此工具你已经下载,即卡Fastboot专用)

</details>

## 刷入MIUI13 For MI8SE

使用MTP将"MIUI 13 For MI8SE"传入手机

点击"安装",选择"MIUI13 For MI8SE",点击刷入并滑动确认

## 可选的额外步骤

~~V我50~~

# 常见问题

我不知道有什么常见问题,如果你需要联络我们,请加入480388122(QQ)

群问题不知道怎么答? 当然是填我辣!(纳兰音韵)

------------

<p><a style="color: inherit; font-weight: normal; text-decoration: none;" href="https://docsify.js.org">Powered by docsify</a></p>

<p><a style="color: inherit; font-weight: normal; text-decoration: none;" href="https://nalanyinyun.ml/">Copyright 2022 Nalanyinyun/Wilderness AllRightsReserved</a></p>
