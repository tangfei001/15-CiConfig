课时206-Allure在Jenkins中的实战和应用

allure的环境搭建:

1. 安装allure的插件

2. 配置安装allure步骤：
  A.系统管理
  B.Global Tool Configuration
  C.找到Allure Commandline安装，点击后,进行安装,建议选择2.4.1版本
  D.点击保存

3.配置allure的保存
  A.系统管理
  B.系统设置
  C.最后找到Allure Report后，进行配置：
              key:WORKSPACE
              value:D:/git/Python/Four/report
  D.点击保存

4.执行后，生成allure的测试报告:
  A.打开job的配置
  B.增加构建后操作步骤中的Allure Report
  C.填写report

5.安装如下python第三方的库：
   pip  install pytest 
   pip install pytest-allure-adaptor
   pip3 install pytest-allure-adaptor

6. 安装第五点的第三方的库成功之后，在构建步骤中选择windows填写如下的信息：
	cd D:/git/github/irainui/testCase                   D:/gitTest/github/pn1/tests
	d:
	python -m pytest  --alluredir ${WORKSPACE}/report

7.执行后，生成allure的测试报告