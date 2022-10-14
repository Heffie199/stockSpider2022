# stockSpider
仅供参考学习
https://www.yuque.com/maiff/vwhwa6/bomg7w



python3 -m pip install easyquotation pandas baostock stock_pandas


安装
python3 -m pip install easyquotation pandas baostock stock_pandas
安装talib
不同系统不一样，参考https://pypi.org/project/TA-Lib/

配置
修改input.txt里的内容，股票代码安装,分割，注意需要加地区编码，sh：上海；sz：深圳。
sz.002241, sh.600900
修改input_params.txt里的内容，第一行macd，第二行rsi，第三行kdj
12,26,9
6,12,24
9,3,3
运行
python3 main.py
注意，如果在非股票交易日运行会返回空数据，如需要测试，需要改下zhibiao.py里

把第十行数据注释掉，11行取消注释改成对应的日期运行就好

输出
会得到当前日期的文件，可以直接用excel打开


===

#####实习
conda create -n your_name jupyter notebook

安装好后，可以通过指令 conda info -e 查看已有环境情况。

安装好环境后，我们可以使用指令激活 jack 环境：

1.activate jack


activate py3-7-1


可以看到，我们的环境由 base 变成了 jack 。

接下来，我们就可以在这个环境里，安装自己想要的第三方库，比如 requests。

2.conda install requests

对于 conda 搜不到的包，也可以使用 pip 安装：

python -m pip -r requirements.txt
在cmd项目目录下Terminal下面执行
pip install easyquotation

生成requirements.txt文件
pip freeze > requirements.txt
安装requirements.txt依赖
pip install -r requirements.txt

打开cmd窗口
cd 到项目目录 pip install -r requirements.txt
3.需要安装的第三方库安装完毕，可使用命令直接打开 Jupyter Notebook：

jupyter notebook


4.pip3 install matplotlib
手动指定
报错提示超时，盲猜一波是安装源连接网络不行，手动指定一波安装源
pip3 install matplotlib  -i https://pypi.douban.com/simple
pip3 install matplotlib  -i https://pypi.mirrors.ustc.edu.cn/simple/

使用
python3.7

直接git或者下载源码包，安装相关依赖，然后运行main.py即可。

git clone https://gitee.com/ailabx/ailabx.git

cd ailabx

pip install -r requirements.txt

python main.py


###导入包
1.同目录
import
2.不同目录
from 包 import类

import sys

import requests

from lxml import etree
# 同一个目录
import utils
import  history_stock_quotes_scrapy
import myDict

from zhibiao import get_data
# 不同目录
import data_viewer
sys.path.append(r'D:\PythonProject\stock-spider')

# from 包 import类
from data_viewer import rightview
rightview.RightTableView

# from myDict import stock_analysis.utils

# from myDict import stock_analysis.utils

# from stock_analysis.utils import myDict

