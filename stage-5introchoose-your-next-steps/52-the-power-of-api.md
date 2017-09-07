# The Power of API

* 網站與其他服務的 server、 machine 溝通的好工具

  

# XML

* 90 後期發明，祖先 SGML\(80s年代發明，Standard Generalized Markup Language\)

* 很像 HTML，XML 格式上比較嚴格

* 差別：XML、XHTML 一定都有 closing tag，沒有 void tags

* HTML 有 specific tags, XML can have whatever arbitrary tag you want
 * 只要命名上讓使用者看的懂



# Parsing XML

* built-in parser in python

* minidom, python library 處理 parsing 的事

* dom = Document Object Model, computer representation of an XML document

* 在 python 中，你的 object 有 list of children, each of children is some sort of tag object which have a name and attribute

* Every time you deal with XML programmatically, you'll see references to a dom

* minisom 適合處理輕量級的 parsing

* Parsing XML 的檔案大，都 gigabytes

  


# JSON

* JSON is a valid Javascript

* You can express in XML , you can express in JSON

* 跟 python 相似，他們的 dict 和 lists 語法相似

* 包含多種 data type 主要放 dict 和 lists


![](https://lh3.googleusercontent.com/Kf2YOdfYuAYe8A4l5dzd3BSYlMPpYSAopfAvBZrC02SDfzriWbQY4cGeYVRv_rLs5VQOs-iEDoqOlFUCPPRVCHOPSzefKsDuXdfWIdgSQ7HZ-GBLmiAhkG85cRRs6cTppAqWLW1W)

  
