# ltwin-idx

https://github.com/hfx1709/ltwin

我的仓库地址：GitHub - hfx1709/ltwin

首先，打开FireBase Studio，地址我不用说了

然后是 创建的时候
![image-20260112043922]https://github.com/6556GHB/ltwin-idx/blob/main/20260112043922.png
按照图上的填就对了，下面那个一定要勾起来

进去之后，左上角菜单，New Terminal，

然后依次执行

bash clean.sh
bash install.sh
相关文件将会在很长时间之后下载完毕，因为archive服务器太烂了，网速很慢，ISO才1G都要等好久

然后虚拟机会自动启动，现在再次新建一个终端，执行

bash vnc.sh
然后右侧工作区第一个按钮，下面展开 BACKEND PORTS，有个5902端口，我们先点进去，然后肯定会报错，没事，我们找到地址，给他最前面的5902改成6001，然后加载出来的网页我们选择vnc.html，连接即可。

然后是Windows安装，这里是tiny10 b4 x64，能用就对了，基于win10 ltsc 2019精简。你到了选择磁盘绝对找不到磁盘，我们load drivers，然后点browse，然后找到带virtio的那个CD，然后选择amd64文件夹，再选择w10，OK。然后就点安装程序右下角那个键载入驱动，然后就能识别到15G的硬盘了。然后win10会装吧？

接着呢，我们不是到了桌面，会自动出现一个压缩程序在那边压缩系统。等他窗口自动关闭，我们打开开始菜单，Windows System文件夹，This PC，然后找到virtio-win盘，点进去最下面那个带x64的msi执行一下就行了，然后显示器驱动和网卡驱动会自动装上。

然后关闭虚拟机，回到脚本那个终端按Ctrl C退出脚本，然后bash chrome.sh，接着进入系统找到chrome那个光盘，怎么找同上，运行Chrome Setup之后，他会自动打开chrome 7.0，接着你菜单按about chrome等他自动更新到chrome 109 32bit之后，你再用Chrome109访问google.com/chrome下载最新版本或者你别的浏览器也可以，然后装完之后关机，最后运行start.sh享用你的vnc吧。

最后说一句话，不要滥用
