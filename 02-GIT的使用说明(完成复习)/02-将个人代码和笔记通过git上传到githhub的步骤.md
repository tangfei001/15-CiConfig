
**将个人代码和笔记通过git上传到githhub的步骤**


注意:将git路径添加到path的环境变量里面
说明:git安装好之后，建议按照git的管理客户端工具:TortoiseGit

# 第一步:在git中查看配置的信息 #

 git config --list  
----------------------------------------------------------------

## 第二步:秘钥的生成-在git中输入 ##:

   第一步: ssh-keygen -t rsa -C "wuya@outlook.com"
           (输入过程中全部按回车键不用管-会自动生成一个本地秘钥)
   第二步(本地目录找秘钥): 
       01:秘钥的地址 C:/Users/lenovo/.ssh/id_rsa.pub 
       02:打开文件,并复制他
   第三步:登录github在里面输入秘钥
      01:个人中心-setting--SSH-and GPG keys--new SSkeys
      02:tiele:随便写
         key:替换内容
   第四步:配置邮箱
       git config --global user.name "wuya"
       git config --global user.email "wuya@outlook.com"

  第五步:查看是否配置好
       git config -list 
-----------------------------------------------------------------------------
### 第三步:github--在github里面创建库(内容为空) ###
 ---------------------------------------------------------------------------    
#### 第四步:本地创建文件 ####
     '''
	  git init-->初始化
      git add .-->提交文件
      git commit -m "备注信息"
      git push--->把本地的代码提交到服务器 (github)
      git pull-->把服务器的代码与本地代码同步
     '''
--------------------------------------------------------------------------
步骤:
     01:在本地目录(自己选择)github-创建目录pn
     02:在pn目录里面右键--Git Bash Here
     03:git命令输入
         git init #初始化
         ls -la   #生成具体目录
     04:吧对应的文件放到pn里面去
     05:git命令  git add .   
                git commit -m "接口测试框架源码"
                git remote add origin https://github.com/tangfei001/pn.git    
                git push -u origin master

     06:在弹出的对话框中输入github的账号和密码
     07:在github的文件创建里面刷新页面
  