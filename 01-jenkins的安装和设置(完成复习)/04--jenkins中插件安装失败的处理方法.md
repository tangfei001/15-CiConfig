**处理-jenkins中插件安装失败的处理方法**

镜像地址查询：
http://mirrors.jenkins-ci.org/status.html


# 第一种处理的思路 #
01:点击Manage Jenkins
02:点击Correct
03:Advanced
04:下拉找到Update Site
05:查看安装失败的插件，在Available里面搜索重装即可
06:安装完成后重启，插件报错消失
------------------------------------------------------------

## 第二种处理的思路:手动下载插件 ##

jenkins插件下载地址：
	http://updates.jenkins-ci.org/download/plugins/

01:点击进入下载页面，点击对应的版本将直接下载

02:在系统管理–管理插件–高级–上传插件即可

03:点击上传，然后它会自动上传及安装，待jenkins重启后插件即生效

