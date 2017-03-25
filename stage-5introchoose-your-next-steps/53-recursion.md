# 5.3 Recursion\(遞迴\)

[完整課程與補充](https://www.udacity.com/course/viewer#!/c-nd000/l-4160599243/m-48532680)

[BNF 語法](https://zh.wikipedia.org/wiki/%E5%B7%B4%E7%A7%91%E6%96%AF%E8%8C%83%E5%BC%8F)解說

"elegant" code

我們會看到你不需要 while，你真正需要的是 procedure\(程序\)，並且以遞迴方式來思考

  


Recursive Definition

[案例](https://www.udacity.com/course/viewer#!/c-nd000/l-4160599243/e-48666077/m-48624660)

分成兩部分

* Base Case

* Starting point, smallest input

* 不用計算

* Recursive Case

* e.g. word = counter + word

  


Ancestor 的[案例](https://www.udacity.com/course/viewer#!/c-nd000/l-4160599243/e-48508431/m-48686622)

[![](https://lh3.googleusercontent.com/Sq8uYVEwoPXWnADaSTYbNlHHVHMErIxucg23dBeV4BOymRsUKOlebNXjIM_fc2DbgWDxseFrVbpIRA2bwPeFuHySaLbij64gR3ObOBonyG34g0yDoDo7XRbfexi7YI-GN0gsH31u)](https://www.udacity.com/course/viewer#!/c-nd000/l-4160599243/e-48508431/m-48686622)

第一行是 Base Case，第二行是 Recursive Case

  


[數學式](https://www.udacity.com/course/viewer#!/c-nd000/l-4160599243/m-48204982)

factorial\(n\)= n \* \(n-1\)...x 1

factorial\(0\) = 1 ，這是 Base Case

factorial\(n\) = n \* factorial\(n-1\)，這是他的函數\(Recursive Case\)

  


Recursive Factorial\(階乘積\)

[說明](https://www.udacity.com/course/viewer#!/c-nd000/l-4160599243/e-48011993/m-48713689)

  


Palindrome（迴文）

* [解釋](http://www.csie.ntnu.edu.tw/~u91029/Palindrome.html)[課程](https://www.udacity.com/course/viewer#!/c-nd000/l-4160599243/e-48230544/m-48714312)

* 倒著唸也通的字串，e.g. 上海自來水來自海上

* [數學式](https://www.udacity.com/course/viewer#!/c-nd000/l-4160599243/e-48230544/m-48624655)，從旁邊向中間檢查

* 要注意 python 的區間，s\[1:-1\] ，是指s\[1\] 到 s\[-2\]

  


* 5.3 Parallel Computing

[HDFS](http://limitedcode.blogspot.tw/2014/10/hdfs-hadoop-distributed-file-system-hdfs.html)- "Hadoop Distributed File System"

MapReduce

* 假設我有一個較大的檔案，讀取時間長

* process data in parallel，把資料分批計算

* [分成兩組](https://www.udacity.com/course/viewer#!/c-nd000/l-4160599243/m-440618653)，Mapper 一組分堆，Reducer一組計算總量

* Mappers

* little programs that deal with a relatively small amount of data

* 平行處理

* 按字母排序 alphabetical

![](https://lh4.googleusercontent.com/B39v_xDDxfV3xlBLp_Z_fSyps8YS92rJtrE8Oa1JAFl0VVLPxN2_R03e-sDbpE06gpgxZoAi13vEG7UuFQKwRu8qkwGaOdYXg2VvZyU5LjtiS1PGmTeVaDF9y9mj_goiYpxtaaax)

* Hadoop deal with the data in the form of key and value

* 所以這些 records 的資料型態就是 key and value

* 在這個案例 key 是 store name, value 是店的銷售額

* 一旦 Mappers 的工作結束, 新的階段\(phase\)：Shuffle 和 Sort 啟動

* Shuffle

* The movement of the intermediate records from mappers to the reducers

* Sort

* The fact that the Reducers will organize these sets of records

![](https://lh3.googleusercontent.com/gTmda9sgqPaUKYB-Ge8QlhU-oHU2qVFW2xTbJ7hpvRqTYmcC_Uzprtbkl-BkBwlX6XLM-RIO0l1Zhpi_yOvLKGH0CegKaib7h1Q5JxlaBvitC50l8HDcycrhmUold9fU_dmADV9w)

  


Reducers work on one set of records at a time

做個總統計：Key（城市）, values（總銷售額）

