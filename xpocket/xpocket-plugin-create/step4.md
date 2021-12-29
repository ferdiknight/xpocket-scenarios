
1.返回用户目录
`cd ~`{{execute}}

2.下载XPocket程序包
`wget https://a.perfma.net/xpocket/download/XPocket.tar.gz`{{execute}}

3.解压
`tar -xvf XPocket.tar.gz`{{execute}}

4.将刚才构建的插件包 xpocket-plugin-demo-0.0.1-SNAPSHOT-jar-with-dependencies.jar 拷贝至XPocket的plugins目录下
`cp /root/xpocket-plugin-demo/target/xpocket-plugin-demo-0.0.1-SNAPSHOT-jar-with-dependencies.jar /root/xpocket/plugins`{{execute}}

5.启动XPocket
`sh xpocket/xpocket.sh`{{execute}}

6.查看刚才实现的插件
`plugins`{{execute}}
如果刚才没有改变插件名称和namespace，那么你现在应该会看到 demoplugin : XPOCKET 这样一个插件，如果你有修改，那么就会看到你修改的相应的插件名称。

7.执行命令(如果你修改了插件名与命令则请修改为对应的插件名与命令)
`demoplugin.example1 test`{{execute}}

8.你可以在这个terminal继续做更多的尝试，或访问 https://xpocket.perfma.com 获取更多信息。
