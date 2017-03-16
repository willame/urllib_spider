# urllib_spider



简单的百科python页面爬取。



对百科的python页的爬虫，慕课网上的学习代码。现在python 版本众多，所以有些语法差异。此爬虫是python 3.5.2 的版本。

spider_main 中的for 循环中的count 可以控制爬取多少个页面。因为某些页面有错误，所以写了异常处理，'here is a bug , jump'。
爬虫原理其实很简单。


1. 下载页面。爬取一个页面，当然要下载吧。

2. 解析。当然解析很多种方法，lxml 和 BeautifulSoup 等等。但是我不会多讲，因为什么框架和库都要自己用的时候，才算掌握。可以写的时候自己去查文档。

3. 存储。解析的页面当然要想办法存储下来吧。可以存在本地的文件下，但是当数据量很大的时候就去学数据库吧。Mysql 和 MongDB都随意。在我现在写的时候也不会数据库。



Now:  讲解结构了。

url_manage.py: url 管理器。毕竟爬取的页面的过多，为了避免重复爬取，定义一个待爬取和一个已爬取的列表。
html_downloader.py：页面下载器。
html_parser.py: 页面解析器。这里用的re正则表达式和BeautifulSoup。建议大家有时间的把基本的正则学会，还是很快的。然后了解最基本的html和css的格式和内容。
html_output.py: 页面输出器。
spider_main: 主函数。调用其他的方法实现的。

我学python一个月，之前没有语言基础，一个月学会基本语法以及Django框架和Scrapy框架。requests库 和 urllib库。只要静下心没什么问题。新手建议不要直接用Scrapy，很优秀的框架，一般用于爬取大型网站。但是在3.X版本还是坑太多。不如用个urllib相当于自己搭建了一个小型的仓库了。


当然爬虫远远不止这些，这只是为了让大家了解爬虫的基本原理。我也在学习，会不定期陆续分享给大家，如何伪造自己的爬虫，如何防止ip被封，如何使用cookie和session。谢谢大家了！
