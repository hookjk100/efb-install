# efb 一键本地部署脚本
---
efb 本地部署脚本 不支持 docker

需要 root 权限运行

```
wget https://raw.githubusercontent.com/shzxm/efb-install/main/install.sh -O install.sh && chmod +x install.sh && bash install.sh
```

目前支持 Centos7 Ubuntu18/20 Debian8/9/10


脚本直接复制自 shzxm 的 [blog](https://blog.shzxm.com) 观看 [手动部署教程](https://blog.shzxm.com/2020/12/31/efb/) 

相关的配置文件修改 [blog](https://blog.shzxm.com) shzxm 也有写

有问题请去https://github.com/shzxm 提问。

---------------------------------------
（2022.7.24有效）：
1.SSH登陆vps
2.root权限
3.执行一键脚本
wget https://raw.githubusercontent.com/hookjk100/efb-install/main/install.sh -O install.sh && chmod +x install.sh && bash install.sh

4. 执行命令：pip uninstall efb-wechat-slave
5.执行命令：pip3 install git+https://github.com/ehForwarderBot/efb-wechat-slave
6. 执行命令：screen -S wechat
7.执行命令：ehforwarderbot
8.用微信扫码，手机上会出现“微信桌面版登入确认”，点击“登入”。（如果图像不完整造成无法扫码，在二维码下面会出现一段网址，类似：https://login.weixin.we.com/qrcode/hghgyghUyt—w==
,把这段网址放入浏览器打开就是二维码，然后迅速用微信扫码登录。）


微信断开，或者需要重启vps后重启服务：
1.登陆服务器ssh
2.reboot
3. screen -S wechat 或者 screen -S tgbot
4. ehforwarderbot
5.点开服务器上显示的http链接，用微信扫描其中的二维码登陆。
6.关闭服务器ssh。




















