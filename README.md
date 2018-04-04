# 功能简介
  * 通过爬取[西刺代理](http://www.xicidaili.com/wn/)上的https代理点，获取可用的https代理点
  * 可自定义timeout的时间，以及将代理点导出至文件
  * 采用多线程的方式（线程数为100），一般耗时3s左右
 
# 使用方法
  * -t 自定义timeout的时间（可选,默认为1s）
  * -h 自定义导出至文件的文件名（可选,默认直接输出）
	
# 一些使用示例
  * 不带参数使用时，直接输出代理节点
```
D:\Code\https-proxy>python proxies.py
('124.193.37.5', '8888')
('119.28.138.104', '3128')
```
  * 获取timeout为1，将数据输出至test.txt文件下
```
D:\Code\https-proxy>python proxies.py -t 1 -f test.txt
('180.168.184.179', '53128')
('120.92.119.187', '10000')
('223.241.79.146', '18118')
('211.159.177.212', '3128')
('124.193.37.5', '8888')
('118.212.137.135', '31288')
('119.28.138.104', '3128')
```
输出至test.txt
```
***********starting Wed Apr  4 16:13:39 2018, timeout is 0.5**************
('180.168.184.179', '53128')
('120.92.119.187', '10000')
('223.241.79.146', '18118')
('211.159.177.212', '3128')
('124.193.37.5', '8888')
('118.212.137.135', '31288')
('119.28.138.104', '3128')
```
