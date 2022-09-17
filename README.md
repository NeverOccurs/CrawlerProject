[## CrawlerProject

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


### 1.1 链家网二手房源（主要更新了这个，对其他项目感兴趣请移步原作者首页）

主要改动了同步爬取，加入了选择区划的功能，可以在某一区划内对价格进行筛选了。
同时略微优化了源代码，适应了新版界面的样式。

同步爬取：[tongbu.py](https://github.com/LMFrank/CrawlerProject/blob/master/LianJia/tongbu.py)（requests+xpath)

异步爬取：[yibu.py](https://github.com/LMFrank/CrawlerProject/blob/master/LianJia/yibu.py)（asyncio+aiohttp+xpath)

有待改进：

1、加入地铁站距离信息。

2、加入学区信息。

3、其他想到再说。

***](https://github.com/NeverOccurs/CrawlerProject/edit/master/README.md)
