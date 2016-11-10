# 一. 安装 Ubuntu
 
 
 ## 1.安装 VMware

(由于之前安装过虚拟机，所以有现成。很简单，下载包直接安装即可)

 ## 2.下载ubuntu

中文网站 [http://cn.ubuntu.com/download/](http://cn.ubuntu.com/download/)  最新版本16.04，按照系统位数下载

 ## 3.开始安装ubantu

   开启VMware，点击  创建新的虚拟机                                         
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片1.png)  
   
   选择 自定义                                                                               
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片2.png)
   
   一直点击  下一步 ，选择  稍后按照操作系统                             
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片3.png)
   
   选择Linux，在弹出的下拉列表中选择 “Ubuntu”                              
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片4.png)
   
   选择想让这个系统放置的地方，尽可能要有 20GB 的剩余空间，按照默认选择，下一步，选择 将虚拟磁盘存储为单个文件
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片5.png)
   
   一直点击 下一步，点击 自定义硬件                                         
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片6.png)
   
   这里供高级用户选读：在左栏选择 “Processors” 后，点击右栏的 “Virtualize Intel VT-x/EPT or AMD-V/RVI” 选项。开启了 CPU 虚拟化功能后您将会获得更佳的虚拟机体验。<b>此为高级功能，一般用户请不要尝试！！！</b>
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片7.png)
   
   这里是供大众朋友们使用的选项，加速3D图形                                    
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片8.png)
   
   <b>这里是必须更改的选项！！</b>请在左栏选择“CD/DVD（IDE）”选项。然后在右栏点击“使用ISO镜像文件”中的 “浏览”按钮，弹出对话框，选择刚才下载的镜像文件，点击“关闭”，会自动保存的           
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片9.png)
   
   配置完成。点击 完成                                                                       
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片10.png)
   
   点击 “开启虚拟机”。注意：安装时请不要插入 U盘！                            
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片11.png)
   
   然而开不了虚拟机，提示<br><b>this kernel requires an x86-64 cpu but only detected an i686 cpu
   unable to boot please use a kernel appropriate for your cpu。</b></br>
   因为必须要在 BIOS 中启用了相关的 CPU 虚拟化功能，否则开启不了虚拟机。
   启用CPU 虚拟化功能：重启笔记本，然后按住F1键，进入BIOS设置，找到Virtual选项，设置成enable，然后保存退出。重启电脑，可以开启虚拟机。
  
   这表明已经在虚拟机环境中，找到中文语言，安装Ubuntu                           
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片12.png)
   
   安装第三方软件                                                                          
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片13.png)
   
   按照默认选择，点击 “现在安装”                                              
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片14.png)
   
   默认                                                                                                 
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片15.png)
   
   默认键盘分布                                                                 
   
   按图片设置，每次进系统需要密码，点击“继续”                                     
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片16.png)
   
   开始真正的安装了，坐等                                                      
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片17.png)
   
   安装完成后，会显示重启系统。重启电脑就ok的。重启之后进入这个界面                 
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片18.png)
   
   输入密码，稍等片刻，就有漂亮的桌面啦                                                       
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片19.png)
   
   可以在软件中心安装自己想要的软件
   
#  二、安装VMwareTools
 
   新建终端，输入sudo apt-get install build-essential，安装build-essential                                  
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片20.png)
   
   获取root权限，输入sudo su，按照提示输入密码
   点击虚拟机，安装VMware Tools。如果已经装过，会提示重新安装                 
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片21.png)
   
   点击 是，刚刚安装了Ubantu系统，CD-ROM默认指向着系统的镜像，要改指向VMware Tools的镜像，点击“是”之后，系统会自动寻找并指向的                                                                           
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片22.png)
   
   在我的电脑中，找到弹出的VMwareTools安装包                                                
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片23.png)
   
   提取出来，（我这里是提取到桌面），此时桌面会多一个文件                                
   下面打开终端，（快捷键Ctrl+Alt+T），然后切换到root用户（切换命令为：sudo su，回车然后会提示你输入当前登录用户的密码，输入成功后即可进入root用户）：                                                                                
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片24.png)
   
   然后以root用户进入到刚刚提取到的vmware-tools-distrib文件夹下，然后输入命令：./vmware-install.pl，然后回车
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片25.png)
   
   上面的操作后就开始安装VMware Tools了，根据其提示输入yes/no，直到出现Enjoy, –the VMware team就表示安装成功了，然后手动重启虚拟机，显示重新安装，也表示安装成功                                                                                                    
   ![图片](https://github.com/Hiooary/Ubuntu/blob/master/images/图片26.png)
   
   
   


 
