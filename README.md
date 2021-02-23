1.食用方法如下 [Usage] :  
		

2.安装git和它的依赖组件  [Install git and dependent packages] 

	root@hostname# apt-get update     
	root@hostname# apt-get -y install git

3.克隆我的仓库  [Clone my .git]

	root@hostname# git clone https://github.com/secorxnm/RTL8125-Driver-for-Proxmox-VE5-6-and-debian.git  

4.切换到目录	  [Change dir]   

	root@hostname# cd ./RTL8125-Driver-for-Proxmox-VE  

5.赋予运行权限   [Chmod]   

	root@hostname# chmod a+x rtl8125_install.sh  

6.运行脚本    [Run script in shell]   

	root@hostname# bash rtl8125_install.sh  

7.等待一会   [Wait for a minutes]...  


8.检查模块是否已安装加载   [Check kernel module is exist it]   

	root@hostname# lsmod | grep 'r8125'   	
	出现 r8125字样即安装成功   [If show 'r8125' that is OK!]
	
	
9.如果出现  modprobe: ERROR: could not insert r8125: Invalid argument，请重启系统再运行一遍脚本即可。
		
[If show modprobe: ERROR: could not insert r8125: Invalid argument appears, please restart the system and run the script again.]        		
	
