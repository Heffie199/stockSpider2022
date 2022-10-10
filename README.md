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

