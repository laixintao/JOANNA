# SHANA

## useage


1. 使用HPUSBFW格式化U盘
1. 使用  grubinst-1.1-bin-w32-2008-01-01安装grub到U盘（安装成功之后，会显示一个Partition table）
	1. 选择磁盘
	2. 不保存原来的mbr
	3. 不引导原来的mbr
	4. 输出详细信息
	5. 启动时不搜索软盘

3. 配置grub
		1. 拷贝 grub4dos-0.4.4-2009-01-11下面的 menu.lst grldr grub.exe 到U盘
		2. 编辑menu.lst


	    map --mem (hd0,0)/haribote.img (fd0)
    	map --hook
    	chainloader (fd0)+1
    	rootnoverify (fd0)

4. 为了防止我们的镜像文件可能不连续所带来的错误，可以使用Defraggler针对这个文件整理一下。

用到的所有软件已经保存到网盘里面。可以在这里下载：
链接：http://pan.baidu.com/s/1bnEu0vt 密码：vpk6
