**10-Jenkins中执行代码模块找不到的解决思路 **

问题:
1:IDE执行,但是CI执行的时候,提示xx模块不存在
2:IDE中提示xx模块不存在


在pycharm中

01:使用os sys的处理思路
02:使用os 和sys的模块进行
03:包与模块的名字不要重复
04:注意模块的命令-不要和关键的第三方库一样
04:pytest == 4.0.2  生成不了报告的原因-版本太高

举例
import os
import sys

base_dir=os.path.join(os.path.dirname(__file),'page')
sys.path.append(base_dir)



