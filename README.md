# QClient

#### 数字货币行情客户端Demo源码
　QClient是C++客户端Demo源代码，用于演示如何连接蓝目行情网关，以统一化的数据格式，从蓝目数字货币行情网关获取各种行情数据。数据货币爱好者可以将此代码结合到自己的策略中，获取多个市场的行情并进行交易。<br>
　蓝目数据提供了全球各大主流数字资产交易所的全部品种的实时交易行情和各类历史数据，供专业的投资机构和个人宽客使用。数据包含了实时数据ticker, 深度数据depth, 各周期历史kline.并且提供了各个交易所的委托下单、委托撤单、交易信息查询等接口。<br>
　目前支持的数字资产交易所包括：bitfinex, kraken, bitstamp, bittrex, okex, huobi, binance, bitmex,zb, poloniex, bithumb. 提供详细的API访问接口文档，以及针对python, C++ 和java 的客户端访问源码。<br>
　[官方网站](https://www.blueye.info)


#### 使用对象
　数字货币数据分析师<br>
　数字货币量化交易的个人或团队<br>
　对数字货币交易感兴趣的机构<br>
　分析行情数据的个人或团队<br>
　正在学习数字货币交易的人<br>
#### 使用前提
　安装visual studio c++开发工具，建议安装vs2017，其他如2010及以上版本，则需要下载对应版本的boost库。<br>
　安装boost 1.67.0。<br>
　
#### 下载安装

1. 下载安装visual studio c++开发工具，以下以vs2017为例，其他版本注意使用boost的对应版本。<br>
略过

2. 下载安装boost库<br>
下载boost 1.67.0 版本，建议使用二进制版本，无需编译。 https://dl.bintray.com/boostorg/release/1.67.0/binaries/
与vc2017匹配的32位版本是： boost_1_67_0-msvc-14.1-32.exe  
选好安装目录，下一步直到结束。

3. 从本账号下载QClient源码

4. 设置vc2017选项（debug版本）<br>
   1. C/C++ | 常规 | 附加包含目录：E:\dev\boost_1_67_0，设置为实际安装目录
   2. 连接器  | 常规 | 附加库目录： E:\dev\boost_1_67_0\stage\lib32-msvc-14.1;
   

5. 编译，运行连接到蓝目行情网关。例如要接收okex的行情: >QClient.exe gw.blueye.info 5001<br>

####  蓝目数字货币行情网关各交易所端口号

		"okex":"gw.blueye.info:5001",<br>
		"huobi":"gw.blueye.info:5002",<br>
		"bitfinex":"gw.blueye.info:5003",<br>
		"bithumb":"gw.blueye.info:5004",<br>
		"binance":"gw.blueye.info:5005",<br>
		"zb":"gw.blueye.info:5006",<br>
		"kraken":"gw.blueye.info:5007",<br>
		"poloniex":"gw.blueye.info:5008",<br>
		"bitstamp":"gw.blueye.info:5009",<br>
		"bittrex":"gw.blueye.info:5011"<br>

