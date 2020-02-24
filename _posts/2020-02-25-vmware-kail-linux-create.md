---
layout: post
title: 在VMware Fusion虚拟机上安装kail linux
tags: kail linux
---
首先，kail linux官网地址[https://www.kali.org/downloads/](https://www.kali.org/downloads/)<br/>
可以直接下载iso版或者VMware版本，都是可以的，下载完成之后就打开VMware虚拟机，
![VMware Fusion新建截图](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-1-41-10.png){:height="50%" width="50%"}
点击新建之后应该会出来这个界面,在这里如果下载的是.iso文件可以点击中间长方形的框[从光盘或映像中安装],VMware文件的话则点击下面第五个选项(创建自定义虚拟机，之后，之后选择操作系统Linux->Debian 10.x 64位就可以，之后和.iso文件都是类似的),之后会打开一个新界面
![VMware Fusion点击新建之后界面](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-1-47-07.png){:heigh="50%" width="50%"}
在这里我因为之前安装过，所以已经有一个文件了，如果没有安装过，或者想安装新的系统，在这里选择按钮(使用其他光盘或光盘映像),之后选择自己下载好的文件.iso文件,点击继续进入下一个界面
![VMware Fusion创建虚拟机界面截图](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-1-52-52.png){:height="50%" width="50%"}
在这个界面选择Linux->Debian系统，因为kail linux就是基于这个系统开发的，在这里我直接安装的最新版10.x 64位，之后下一个界面
![VMware Fusion选择操作系统界面](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-1-59-30.png){:height="50%" width="50%"}
这里两个选项，哪个都是可以的，只是我查了后说UEFI固件接口系统启动更快，容错率更高，所以我就选UEFI接口了，之后继续就可以了。
![VMware Fusion选择固件类型界面](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-2-04-32.png){:height="50%" width="50%"}
之后如果想要更改设置界面则选择你安装的虚拟机右键->设置
![VMware Fusion虚拟机设置](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-2-10-36.png){:height="50%" width="50%"}
在这个界面中处理器和内存是用来改变分配给虚拟机的内存大小和处理器数量的，而硬盘就是更改分配给硬盘的大小的了。这些根据自己需要的来，注意不要比默认的小就好了。
![VMware Fusion虚拟机设置](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-2-18-11.png){:height="50%" width="50%"}
之后启动虚拟机
![VMware启动kail linux界面](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-2-22-59.png){:height="50%" width="50%"}
第一个选项是安装有GUI的界面，第二个就是只有命令行的了，看自己需要，如果是刚接触linux的话推荐安装第一个，之后等待一段时间，之后界面中选择语言，国家，键盘映射等，这个很简单。再次等待一段时间后，需要填写主机名(相当于这台电脑的名字,默认就行),
![kail linux主机名填写](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-2-35-33.png){:height="50%" width="50%"}
下一个域名直接为空,点击继续,首先是设置用户真实名称(我是随便填的)
![kail linux真实名称](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-2-38-57.png){:height="50%" width="50%"}
然后是设置用户和密码(需要注意的是新版的kail linux这里设置的是非root用户，需要root用户的话可以在进入后设置，后面有写怎么设置)
![kail linux用户名设置](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-2-42-15.png){:height="50%" width="50%"}
![kail linux密码设置](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-2-43-25.png){:height="50%" width="50%"}
之后再次等待一段时间，然后是磁盘分区，选择使用整个磁盘
![kail linux磁盘分区](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-2-47-54.png){:height="50%" width="50%"}
要分区的磁盘
![kail linux要分区的磁盘](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-2-50-50.png){:height="50%" width="50%"}
分区方案
![kail linux分区方案](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-2-53-35.png){:height="50%" width="50%"}
结束分区
![kail linux结束分区](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-2-56-27.png){:height="50%" width="50%"}
然后这里选择"是"，将改动写入磁盘
![kail linux分区写入磁盘](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-2-58-20.png){:height="50%" width="50%"}
之后等待安装系统，然后选择http代理，没有的话留空
![kail linux http代理](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-3-01-31.png){:height="50%" width="50%"}
之后配置软件包管理，如果遇到失败，可以直接选"否"
![kail linux软件包管理](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-3-04-38.png){:height="50%" width="50%"}
软件选择，第一个选项有新版的桌面，所以我就选择了
![kail linux软件选择](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-3-16-46.png){:height="50%" width="50%"}
之后等待一段时间就安装完成了，进入系统时就用自己安装时的用户和密码就可以了<br/>
进入系统后有几个问题需要解决，而解决这几个问题首先需要root账户
```code
sudo passwd root

#kail的密码： #当前用户的密码<br/>
#新的密码:    #输入root用户的密码<br/>
#重新输入新的密码:   #再次输入root用户的密码<br/>
```
之后就可以切换到root账户了<br/>
```code
su root
```
接下来的问题是中文乱码问题<br/>
```code
dpkg-reconfigure locales
```
接下来弹出这个界面,然后选择"en_US.UTF-8 UTF-8"和"zh_CN.UTF-8 UTF-8",按空格选中，回车
![kail linux选择语言界面](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-3-58-42.png){:height="50%" width="50%"}
然后将en_US.UTF-8选为默认(现在会变成英文字符，之后安装桌面后再将zh_CN.UTF-8改为默认)
![kail linux语言默认界面](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-4-37-03.png){:height="50%" width="50%"}
之后重启系统
```code
#重启
reboot
```
然后需要更新源，安装中文字体
```code
vim /etc/apt/sources.list
```
#阿里云
deb http://mirrors.aliyun.com/kali kali-rolling main non-free contrib<br/>
deb-src http://mirrors.aliyun.com/kali kali-rolling main non-free contrib<br/>
#清华大学<br/>
deb http://mirrors.tuna.tsinghua.edu.cn/kali kali-rolling main contrib non-free<br/>
deb-src https://mirrors.tuna.tsinghua.edu.cn/kali kali-rolling main contrib non-free<br/>
然后是这两个源，随便用阿里源或清华都都可以
最后输入
```code
#更新源和软件，如果没有效果可以reboot重启
apt-get update && apt-get upgrade && apt-get clean
#安装中文字体
apt-get install xfonts-intl-chinese ttf-wqy-microhei
```
然后是没有GUI桌面的问题，kail linux 19.4版本后有一个xfce桌面，消耗性能更少
```code
apt install x-window-system-core xfce4
#安装完成后重启看看吧
reboot
```
进入桌面后如果是英文的，可以再打开终端，输入命令
```code
dpkg-reconfigure locales
```
将zh_CN.UTF-8选为默认后，reboot重启就ok了
![kail linux xfce桌面](/assets/image/2020-02-25-vmware-kail-linux-create/2020-02-25-5-40-31.png){:height="50%" width="50%"}