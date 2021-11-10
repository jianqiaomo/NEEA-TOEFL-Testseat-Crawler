## NEEA托福考位爬虫 Getting Started with NEEA TOEFL Testseat Crawler

本文档简要介绍了NEEA托福考位本地爬虫的使用方法。
This document provides a brief intro of the usage of NEEA TOEFL Test Seats Selenium Crawler.

### 动机 Motivation
NEEA 托福考位网站正在提供着不便的服务。在寻找考位时，我们需要按每个日期，每个城市一个个地搜索考位，
这为那些想尽快找到测试座位的人带来了无法忍受的体验。

<div align="center">
  <img src="https://s1.ax1x.com/2020/07/18/UcfnqP.gif"/>
</div>

为什么不直接以表格形式显示所有考位？

[NEEA TOEFL](https://toefl.neea.cn/) Test Seat website, supported by Chinese National Education 
Examinations Authority (NEEA), is providing an inconvenience service. When looking for a test seat, 
we need to search date by every date, every city, which brings an intolerable experience for those 
who just want to find a test seat ASAP. Why not display the form of all the test seat?

### 安装要求 Requirements
- Firefox [mozilla geckodriver](https://github.com/mozilla/geckodriver/releases) v0.26.0
    - [How to install webdriver](https://www.cnblogs.com/LY-CC/p/11068244.html)
- [Firefox](https://ftp.mozilla.org/pub/firefox/releases/) ≥ 60
- pip install selenium
#### 安装方式 Install
- Firefox mozilla geckodriver: the default geckodriver path is "C:\Program Files\Mozilla Firefox\geckodriver.exe". 
If you want to set your executable path, please use **--webdriver_path='your path'** to start.

- 默认Firefox mozilla geckodriver是安装在"C:\Program Files\Mozilla Firefox\geckodriver.exe"路径中，如果你希望使用其他路径，
请使用 **--webdriver_path='your path'** 来启动爬虫。

### Get start
default start
```
python crawler_toefl.py --username='NEEA ID number' --password='password'
```
When finished, you can get a .csv form file. 爬虫完成后将得到.csv表格文件。

<div align="center">
  <img src="https://s1.ax1x.com/2020/07/18/Uch9Qs.png"/>
</div>

### Todo:
1. faster, test time is 30 min 爬虫速度太慢了, 爬完全部数据目前需要30分钟
2. headless mode 无界面模式怎么绕开反爬虫?
3. Anti anti-crawler when click the 'search seats' button 怎么绕开反爬虫?
4. online crawler (use a server) 在线爬虫(服务器)
5. different modes 用户定制化爬虫

### Acknowledgement
This idea is initially coming from https://www.jianshu.com/p/2541d918869e, thanks!  
