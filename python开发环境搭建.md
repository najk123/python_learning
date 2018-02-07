### python开发环境搭建
---
#### 1.工具列表
* centos、windows
* mobaxterm
* pycharm

---
#### 2.mobaxterm的安装及使用
  
---
#### 3.pycharm的安装及使用
  
---
#### 4.pip安装模块
  
---

  在在centos上将pycharm通过mobaxterm投射到windows上时遇到一点问题，结果投射失败。后面找到了[解决办法](http://blog.csdn.net/ipaomi/article/details/78526643?locationNum=5&fps=1)，我的是centos上/etc/ssh/sshd_config的配置问题。修改配置后重启服务 ```service sshd restart``` 。建立软连接 ```ln -s /root/pycharm-5.0.6/bin/pycharm.sh /usr/sbin/pycharm``` ,可以在任意路径下通过命令```pycharm```直接启动了。
  最终效果是，在centos上输入```pycharm```,在windows上出现pycharm启动画面及界面。
