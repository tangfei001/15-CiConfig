**jenkins和jmeter工具的整合说明**


# 01:jenkins中如何运行jmeter文件 #

步骤:
01:新建item--输入任务名称:jmeter5.2.1-选择Freestyle project

02:在打开的界面中
    01:描述可以不写
    02:选择Discard old builds(丢弃旧的构建)-保持构建的最大个数(输入6)
    03:构建-选择-Invode Ant ---选择高级
       Build file目录: G:/apache-jmeter-5.2.1/tests/build.xml

03: 返回jenkins页面-点击立即构建

-------------------------------------------------------------------------
## 02:在jenkins中生成HTML测试报告的步骤 ##

设置页面

01:构建后操作-Pblish HTML report-选择[高级]

02:HTML directory to archive: G:\apache-jmeter-5.2.1\tests\report\html
   Index page[s]: *.html

03:点击保存

04:回到页面点击-立即构建-结束后就能生成对应的HTml文件,进行查看
-------------------------------------------------------------

### 03:在jenkins中生成性能测试报告的步骤 ###

设置页面:

01:构建后操作-选择Publish Performance test result report--选择高级

02:Source data files (autodetects format): G:\apache-jmeter-5.2.1\tests\report\jtl\*.jtl
