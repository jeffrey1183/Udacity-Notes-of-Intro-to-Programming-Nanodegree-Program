  


# 5.2 The Power of API

[例子](http://ascii-chan-ipnd-complete.appspot.com/)：猜出 User 的位置，把你 pin 在地圖上

  


功能

* new data structure \(XML\) and a new programming tool \(APIs\).

* 網站與其他服務的 server、 machine 溝通的好工具

![](https://lh6.googleusercontent.com/VXMBpX8ITVNGve6PQW2xu03AfwhesZ-rLdWiPAgG3fElTujg4B_ipBAw0cWjIKvxh80paNB_72lykbR3MbTb5cOyzUQh5B0M60wnljCC1ZCzDb3WcN0XuphqARtN6UWJ6HmnIqKi)

  


[Telnet](https://zh.wikipedia.org/wiki/Telnet)

  


Making basic request with urllib

* [還不了解](https://www.udacity.com/course/viewer#!/c-nd000/l-4191238688/m-48258977)

  


XML

電腦與電腦間的溝通

* HTML 不適合，怕東漏西漏 tag

  


* 90 後期發明，祖先 SGML\(80s年代發明，Standard Generalized Markup Language\)

* Have a regular way of expression data between computer systems

* Easy to parse

* 很像 HTML，祖先一樣

* 差別：XML、XHTML 一定都有 closing tag，沒有 void tags\(e.g. &lt;br&gt;\)

* HTML 有 specific tags, XML can have whatever arbitrary tag you want

* 只要命名上讓使用者看的懂

* XML 格式上比較嚴格

* 第一行 document type

* If you want a tag that has no content in XML

* 你可以 &lt;br/&gt; 把 / 加在大於前面，蠻常見

* 這種 doc type 其實叫 xhtml

* 表示我的 HTML documents is actually going to be valid XML instead of doing void tag with no closing slash

* [說明](https://www.udacity.com/course/viewer#!/c-nd000/l-4191238688/e-48381415/m-48737027)

* wiki 的頁面有 xhtml、html，方便在 server 間用 XML 轉換

  


Parsing XML

* built-in parser in python

* minidom, python library 處理 parsing 的事

* dom = Document Object Model, computer representation of an XML document

* 在 python 中，你的 object 有 list of children, each of children is some sort of tag object which have a name and attribute

* Every time you deal with XML programmatically, you'll see references to a dom

* minisom 適合處理輕量級的 parsing

* Parsing XML 的檔案大，都 gigabytes

  


JSON

* JSON is a valid Javascript

* You can express in XML , you can express in JSON

* 跟 python 相似，他們的 dict 和 lists 語法相似

* 包含多種 data type 主要放 dict 和 lists

  


![](https://lh3.googleusercontent.com/Kf2YOdfYuAYe8A4l5dzd3BSYlMPpYSAopfAvBZrC02SDfzriWbQY4cGeYVRv_rLs5VQOs-iEDoqOlFUCPPRVCHOPSzefKsDuXdfWIdgSQ7HZ-GBLmiAhkG85cRRs6cTppAqWLW1W)

  


Parsing JSON

* [開始 parse](https://www.udacity.com/course/viewer#!/c-nd000/l-4191238688/m-48717271)

* 看一個網站的 json 檔案

* 寫法：[https://www.reddit.com/.json](https://www.reddit.com/.json)

* 也可以換成 .xml ，看 xml

* [https://www.reddit.com/.xml](https://www.reddit.com/.xml)

  


API

* 如果你要別的網站的內容，poking around to their APIs （戳他們的 API）

* e.g. 找 twitter API 文件

使用別人的 API，要有良心

![](https://lh5.googleusercontent.com/C2soiohuvoO3uqyasOEq1hujwiz-pmZ2rp-gcJioKQw7qDkOgZW9UsekxuAqPgiAYn9AkPvBz4sUX2a-TLPmB-2Rh6McRhOe6_yrsdpd3MOhEyt1chVri3eo_yvcB4Tj4mcuz-U5)

* python 可搭配 time.sleep\(\) method[here](http://docs.python.org/library/time.html#time.sleep)

  


  


[![](https://lh3.googleusercontent.com/bjXa3vL9wPU-cYHJN0FtY-ep4FUwpf9_SNG0DmSNW89L7Mqu_fT9fc1CS_9R0v0d9DX_AOucIdk0vDlo7-0EEFh3s2GY1jANxbeFS2ArzvtwuHSiUJkVM4q6gzfl-R0CQ7ClwIUf)](http://docs.python.org/library/time.html#time.sleep)

SOAP - Microsoft

* based on XML

* protocol for communicating with two machines

* 缺點 complicated

* HTTP + JSON， whole package

* Protocol Buffers 和 Thrift 以 JSON

Protocol Buffers - Google

* Encoding different types of data for sending it over wire

Thrift - Facebook

* 最後一項，hard to just use JSON

  


ASCII Chan Program

![](https://lh4.googleusercontent.com/mMhkDMbWzaIQrCKWTXAmjiR7CR9-aQzkLhDYovTEBirx-Cnfem-xyIw5WWPhFxvUqFBigI9rjgtPHenJr4bW-0KVaCH-s1zuqf0cz3Np1xWEe_cK1MyhiaQVOf9Pf6i9wJdZrGUr)

難在程式邏輯，後面的都還不懂

[https://www.udacity.com/course/viewer\#!/c-nd000/l-4191238688/m-4080748764](https://www.udacity.com/course/viewer#!/c-nd000/l-4191238688/m-4080748764)

