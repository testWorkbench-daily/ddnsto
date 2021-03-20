## 玩转应用中心
1.登录到https://www.ddnsto.com/。

2.通过前面的详细教程，已经配置好穿透。

3.右上角就点击远程应用，就能看到丰富的远程应用。

4.接下来我们就来玩转这些应用。

  ![CloudApp](./cloudapp/cloudapp1.jpeg)
  
  ![CloudApp](./cloudapp/cloudapp.jpeg)

## 1.玩转Aria2远程下载

### Aria2配置：OpenWrt
1.首先确定你的路由等设备安装好了Aria2。
  
2.启用Aria2，RPC认证方式选令牌，然后自己输入一段英文数字乱码当作密钥，并复制下来(后面要用)，然后设置好下载目录，提交。
   
  PS：OpenWrt的RPC认证方式可选无，直接提交启用，然后跳转到“远程配置”，去设置远程下载。 
  
  ![Aria2](./cloudapp/cloudapp-aria2-2.jpeg)
  
  ![Aria2](./cloudapp/cloudapp-aria2-1.jpeg)

3.启用成功后，点击AriaNg控制台，并进入。

  ![Aria2](./cloudapp/cloudapp-op.jpeg)

4. 进入AriaNg控制台，会发现状态未连接，那我们就来设置：先点击AriaNg设置，再点击RPC，地址填入路由IP，再填入密钥，重载界面就发现已经连接了。
 
  ![Aria2](./cloudapp/cloudapp-aria2-lede4.jpeg)

  ![Aria2](./cloudapp/cloudapp-aria2-lede5.jpeg)  
  
5.然后跳转到“远程配置”，去设置远程下载。 


### Aria2配置：KS LEDE
1.在酷软中心安装Aria2。

  ![Aria2](./cloudapp/cloudapp-aria2-lede1.jpeg)

2.设置好下载目录，并启用Aria2和开启RPC访问密钥，提交以后复制密钥(后面要用)。

  ![Aria2](./cloudapp/cloudapp-aria2-lede2.jpeg)
  
3.启用成功后，点击AriaNg控制台，并进入。

  ![Aria2](./cloudapp/cloudapp-aria2-lede3.jpeg)

4. 进入AriaNg控制台，会发现状态未连接，那我们就来设置：先点击AriaNg设置，再点击RPC，地址填入路由IP，再填入密钥，重载界面就发现已经连接了。
 
  ![Aria2](./cloudapp/cloudapp-aria2-lede4.jpeg)

  ![Aria2](./cloudapp/cloudapp-aria2-lede5.jpeg)

5.然后跳转到“远程配置”，去设置远程下载。   

  
### Aria2配置：KS 梅林
1.在软件中心安装Aria2。

  ![Aria2](./cloudapp/cloudapp-aria2-ml1.jpeg)

2.开启Aria2和远程穿透连接，然后会自动配置RPC。
  
  ![Aria2](./cloudapp/cloudapp-aria2-ml2.jpeg)

3.点击RPC设定，然后复制RPC密码/token(后面要用)。
  
  ![Aria2](./cloudapp/cloudapp-aria2-ml3.jpeg)

4.然后跳转到“远程配置”，去设置远程下载。

   
### Aria2配置：群晖

TODO

### Aria2配置：威联通

TODO

### Aria2配置：爱快/Docker

TODO

### Aria2配置：老毛子Padavan

TODO

### Aria2配置：ReadyNAS
 
TODO 

 
### 远程配置  
1.在ddnsto可用应用列表中点击添加远程Aria2。

  填入RPC地址(格式为：路由IP:6800，比如http://192.168.2.2:6800/jsonrpc)
  
  password为前面复制的RPC密码/token(如果没RPC密码可不填，比如OpenWrt可不设置，就能远程)。
  
  ![Aria2](./cloudapp/cloudapp-aria2-3.jpeg)

2.在已添加中找到刚添加的远程应用，点击即可进入Aria2操作界面。
  
  ![Aria2](./cloudapp/cloudapp-aria2-4.jpeg)

  ![Aria2](./cloudapp/cloudapp-aria2-5.jpeg)

3.Aria2操作界面新建填入要下载资源的地址即可远程下载了。 
 
  ![Aria2](./cloudapp/cloudapp-aria2-6.jpeg) 
  
  ![Aria2](./cloudapp/cloudapp-aria2-7.jpeg)
   
  
## 2.玩转远程SSH
1.首先确定你的路由等设备开启了SSH。

2.在可用应用列表中点击添加远程SSH。

3.在弹出窗口写入应用名称，设备IP、设备登录用户名/密码等信息。

  PS：端口一般不需要改，除非你自己改了！
  
  ![SSH](./cloudapp/cloudapp-ssh1.jpeg)  

4.在已添加中找到刚添加的远程应用，点击即可进入设备的SSH。  
  
  ![SSH](./cloudapp/cloudapp-ssh2.jpeg)  
	
  ![SSH](./cloudapp/cloudapp-ssh3.jpeg)
 
 
## 3.玩转远程Telnet
1.首先确定你的路由等设备开启了Telnet。

2.在可用应用列表中点击添加远程Telnet。

3.在弹出窗口写入应用名称，设备IP、设备登录用户名/密码等信息。

  PS：端口一般不需要改，除非你自己改了！
  
  ![Telnet](./cloudapp/cloudapp-telnet1.jpeg)  

4.在已添加中找到刚添加的远程应用，点击即可通过Telnet进入设备的。  

  ![Telnet](./cloudapp/cloudapp-telnet2.jpeg)

  
## 4.玩转Windows RDP远程
1.首先在被控制的电脑上启用远程桌面。

Win10：设置——系统——远程桌面——启用远程桌面  

  ![Windows远程](./cloudapp/cloudapp-rdp1.jpeg)

Win7：右键我的电脑——属性——左边侧栏高级系统设置——远程，在下方“远程桌面”方框下勾选“允许远程连接到此计算机”
  
  ![Windows远程](./cloudapp/cloudapp-rdp2.jpeg)

2.查看被控制的电脑的IP和用户名/密码。

“开始键+R”一起按，出来窗口输入“cmd”回车，出来终端窗口，输入“ipconfig”回车；

  ![Windows远程](./cloudapp/cloudapp-rdp3.jpeg)

  ![Windows远程](./cloudapp/cloudapp-rdp4.jpeg)

确定自己是以太网(网线接入)还是WLAN(WiFi)，找到ip地址，记住。(查看IP方法很多，不一定是这一种)  
  
  ![Windows远程](./cloudapp/cloudapp-rdp5.jpeg)

用户名和密码：控制面板——用户账户——用户账户，能看到当前的用户名，密码是自己设置的。

PS：某些Win10用户是用的微软帐号，没启用本地帐号，那么就使用微软帐号和密码。

或者简单点：开机登录的时候，显示的就是用户名。

   ![Windows远程](./cloudapp/cloudapp-rdp6.jpeg) 
 
3.在ddnsto可用应用列表中点击添加远程RDP，填入被控电脑的IP，用户名，密码等信息。

   ![Windows远程](./cloudapp/cloudapp-rdp7.jpeg) 
   
4.在已添加中找到刚添加的远程RDP，点击即可进入进入RDP，操控远程电脑。 

   ![Windows远程](./cloudapp/cloudapp-rdp8.jpeg)  
   
5.相关提醒：

  a.被控电脑必须是在设置好穿透(ddnsto)的网络设备下
  
  PS：比如我路由器上设置好了ddnsto，我电脑是连接的我的路由器上网的
  
  如果是你想控制你朋友的电脑，而你朋友的电脑就是普通的接入网络，也没ddnsto，那么是不可控的
  
  b.被控电脑必须是开机状态，且没进入休眠状态

  c.确保被控电脑接入网络，且网络是通畅的
  
  
## 5.玩转远程VNC

  TODO
 
 
## 6.玩转远程开机

  TODO