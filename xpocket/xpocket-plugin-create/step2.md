
1.使用XPocket发布的项目原型构建一个Maven项目
`./apache-maven-3.5.4/bin/mvn archetype:generate -B -DarchetypeGroupId=com.perfma.xlab -DarchetypeArtifactId=xpocket-plugin-archetype -DarchetypeVersion=2.0.1-RELEASE -DgroupId=com.perfma.xlab -DartifactId=xpocket-plugin-demo -Dversion=0.0.1-SNAPSHOT -Dpackage=com.perfma.xlab.plugin.demo`{{execute}}

2.检查项目结构
`cd xpocket-plugin-demo`{{execute}}
`ls`{{execute}}

3.按你自己的需求修改插件定义文件
`cd /root/xpocket-plugin-demo/src/main/resources/META-INF`{{execute}}
`vim xpocket.def`{{execute}}

4.修改完成退出编辑
`:wq`{{execute}}

5.查看核心逻辑实现文件
`cd /root/xpocket-plugin-demo/src/main/java/com/perfma/xlab/plugin/demo/`{{execute}}
`ls`{{execute}}

6.ExampleXPocketPlugin.java 主要用于管理插件的整体生命周期，ExampleXPocketCommand.java 主要用于实现一个或多个命令的核心执行逻辑，修改一下命令实现
`vim ExampleXPocketCommand.java`{{execute}}

7.修改完成退出编辑
`:wq`{{execute}}
