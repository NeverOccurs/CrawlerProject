## CrawlerProject

* [1.1 链家网二手房源](https://github.com/LMFrank/CrawlerProject/tree/master/LianJia)
* [1.2 Wikipedia](https://github.com/LMFrank/CrawlerProject/tree/master/Wikipedia)
* [1.3 BaiduAPI](https://github.com/LMFrank/CrawlerProject/tree/master/baidumapapi)
* [1.4 爬取虎扑步行街](https://github.com/LMFrank/CrawlerProject/tree/master/Hupu)
* [1.5 链家网租房爬虫项目（Scrapy+异步MySQL）](https://github.com/LMFrank/CrawlerProject/tree/master/lianjia_scrapy)
* [1.6 房天下新房、二手房爬虫项目（Scrapy-Redis分布式爬虫)](https://github.com/LMFrank/CrawlerProject/tree/master/fangtianxia_scrapy_redis)
* [1.7 微信公众号（通过代理池爬取）](https://github.com/LMFrank/CrawlerProject/tree/master/Wechat)
* [1.8 爬取网页转换成pdf](https://github.com/LMFrank/CrawlerProject/tree/master/html2pdf)
* [1.9 下载bilibili视频](https://github.com/LMFrank/CrawlerProject/tree/master/bilibili_video)
* [1.10 本地保存微信公众号文章](https://github.com/LMFrank/CrawlerProject/tree/master/%E5%BE%AE%E4%BF%A1%E5%85%AC%E4%BC%97%E5%8F%B7%E6%96%87%E7%AB%A0%E8%8E%B7%E5%8F%96)

**NOTE:**

1. 开发环境：Win10(WSL-Ubuntu、VMWare-Ubuntu Server 18.04) + Anaconda3 + PyCharm(VSCode) + Cmder + XShell
2. WSL环境的搭建可参考我写的博文：[打造Win10+WSL开发环境【图文】](https://blog.csdn.net/LMFranK/article/details/100214551)
3. ~~VSCode Insider版本实现win10下远程连接WSL编写代码更加方便~~，Pycharm更好用
4. WSL的文件共享推荐XShell，VBox直接使用共享文件夹。如果使用Pycharm，可以直接进入tools-Deployment-configuration，创建sftp连接
5. 终端强烈推荐Cmder，可以直接进入WSL环境
6. 所有项目的包依赖集合在[requirements.txt](https://github.com/LMFrank/CrawlerProject/blob/master/requirements.txt)，其中因为部署在linux服务器上，所以我删除了pywin32包及mkl包，有需求可以自行添加

**Go版爬虫链接**：[https://github.com/LMFrank/Go_Crawler](https://github.com/LMFrank/Go_Crawler )

***


### 1.1 链家网二手房源（主要更新了这个）
链家网的显示方式为每页30条房源数据，最多显示100页，即3000条。因此，我使用二分法切割价格区间，从而得到完整数据。

加入了选择区划的功能，可以在某一区划内对价格进行筛选了。
同时略微优化了源代码，适应了新版界面的样式。

同步爬取：[tongbu.py](https://github.com/LMFrank/CrawlerProject/blob/master/LianJia/tongbu.py)（requests+xpath)

异步爬取：[yibu.py](https://github.com/LMFrank/CrawlerProject/blob/master/LianJia/yibu.py)（asyncio+aiohttp+xpath)

有待改进：

1、加入地铁站距离信息。

2、加入学区信息。

3、其他想到再说。

***
