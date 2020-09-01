**课时189-Jenkins的介绍与安装**

A、到https://jenkins.io/download/下载	  
B、jenkins.war
	      java -jar jenkins.war    
C、下载tomcat,解压，把jenkins.war放到tomcat的webapps目录下
D、然后到tomcat的bin目录下  启动startup.bat
E、监听的端口默认是8080:
		  netstat -ano | findstr "查询的端口"
		  tasklist | findstr "PID"
F、http://localhost:8080/jenkins
		  a、请你输入密码的提示
			 win:C:\Users\Administrator\.jenkins\secrets,打开initialAdminPassword
			 linux:/root/.jenkins/secrets,打开initialAdminPassword
		  b、安装插件,所有的都选择
		  c、安装插件成功之后,点击完成按钮,就会跳转到jenkins的首页
