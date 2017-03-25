**4.8 Databases**

**Store and retrieve some data to user，**[**簡介**](https://www.udacity.com/course/viewer#!/c-nd000/l-4195258602/m-48712317)

[![](https://lh6.googleusercontent.com/99wLggn8qHpBENnP6yAWE7gI-f8zq29bqPBQTxEYUWlGD9qhFmMNklQI6e_worwOlkIIXR57ktDau_9HGMwjHweNYAmlme40_vhqbCEp9J6PvTsCVQrlZdeRftw8FJ750z4MmMYm)](https://www.udacity.com/course/viewer#!/c-nd000/l-4195258602/m-48712317)

**  
**

**Columns of database**[**說明**](https://www.udacity.com/course/viewer#!/c-nd000/l-4195258602/m-48734217)

[![](https://lh6.googleusercontent.com/BdMrsrT8tB_h33ZFf0sr0YAXWyA6oP1r8I7HUDGV13bUp0lLX0FL8p-HJYGoPCV8iu7gXt3H78ZbW4BSr0_OkfYpddTtB2lkAJZbn5R7-wsOfCqPeaHP5tYuwibxtwJIm1KmZasH)](https://www.udacity.com/course/viewer#!/c-nd000/l-4195258602/m-48734217)

**ID column 最重要**

* **一般是 integer 或 string**

**Vote column**

* **number of votes on this link**

**User column**

  
**  
**

**  
**

* **還會有專門的 user table**

**Date column**

* **此例使用 date type，不一定都支援**

[**Lambda**](http://falldog7.blogspot.tw/2009/07/python-lambda.html)

**  
**

**證明 querying a database by writing Python code is very hard，又慢又容易錯，又蠢（**[**說明**](https://www.udacity.com/course/viewer#!/c-nd000/l-4195258602/e-48666066/m-48720182)**），幸好有 database，處理大量資料的好幫手**

**  
**

**Types of Databases**

![](https://lh4.googleusercontent.com/XXeYVa7coHBn6NM4VtJzslyuezTML4QokjIZM9Kv-Ji9XhcGGJ5I0BJfsK0uqrjy1zl4bOT-1Lv4U_rIuPDkqshZtG5zlf4rzvlPnt3l7tWohH4GU1ge-RgD5yEYs58RoYG-WGWR)

**  
**

**SQLite - 較省容量，lightweight**

**Oracle 買下 MySQL 很久，但還是讓他免費唷**

**這些資料庫都 work with tables and use a language SQL to manipulate**

**其他**

* **Google App Engine Datastore**

* **Dynamo by Amazon**

* **NoSQL**

* **Mongo**

* **Couch**

* **改善 MySQL 他們的缺點**

**  
**

**Data type called the "named tuple"**

* **This is very similar to a Python Class in that it lets you refer to the properties of something by their name. You can read more about named tuples in**[**this thread on stackoverflow**](http://stackoverflow.com/questions/9872255/when-and-why-should-i-use-a-namedtuple-instead-of-a-dictionary)

**Here is more**

[**information**](http://docs.python.org/2/library/collections.html#collections.namedtuple)

**on named tuple used in this exercise.**



**  
**

**SQL**

* **A language for expressing queries**

**  
**

![](https://lh4.googleusercontent.com/bnoFQqF2f1i9vJvZYrYkLMe77FZJ35sVMJd_RyXqu4RtZfOUVJWnKIGudZQSUV9XqKyieis5mkQwgzMZ5WKK6d-8nrtr8nmgyykTF26YHfBGN4bCkE_VYWg1gIKTZupzPjaZGCld)

**分成三部分：**

**Select Clause**

* **\* 代表全部，可以換成 url,title**

**From Clause**

* **where we fetch data from**

**Where Clause**

* **They are constraints which rows from our table to return**

* **他可能很長**

**  
**

**Import SQLite3 in Python**

* [**說明**](https://www.udacity.com/course/viewer#!/c-nd000/l-4195258602/e-48666068/m-48632774)

* **c = cursor \( a position in the database\)**

**  
**

* **def query\(\)**

* **c=db.excute\("select \* from links"\)**

* **result = c.fetchall\(\)**

* **return result**

* **\# load all of the data out of database into the list of results**

**  
**

**補充: fetchone\(\) ，returns the first result**

**  
**

**Iterate our cursor in tuple into link object**

* **We get back the result one by one from database, we get them back as a tuple, not as our link object**

* **Tuple is a reserved word**

* **但我們實際要的是 link objects**

* **做法**

* [**說明**](https://www.udacity.com/course/viewer#!/c-nd000/l-4195258602/e-48666068/m-48632774)

* **link = Link\(\*link\_tuple\)**

* **是一個 python 的語法**

* **passing all of the parameters in this tuple as arguments to a link object**

**  
**

**Creating this table**

![](https://lh6.googleusercontent.com/7epcf1C6K68eN4-MSFt9a4JObOXI1QcFgbpSa17ASON6x1lhOdS4wlcq3Yj3ddeMcj0xDg9UYvT3roshYq0FrMv3DsvyZ6EiBu1s5b3sGSSrIJGYe51XzdcdLIdn7et0c5sxjDb9)

**  
**

**Where Clause - Advanced**

* **Selcet \* From links where votes&gt;23 and ID=5**

* [**說明**](https://www.udacity.com/course/viewer#!/c-nd000/l-4195258602/m-48673662)[**實作**](https://www.udacity.com/course/viewer#!/c-nd000/l-4195258602/e-48538418/m-48733149)

[![](https://lh6.googleusercontent.com/N9Tq5U01Ffky2fSw-w6mUbIece--z5eYACHq-728qyAwdU7v9Bnb612O3udgsi-jkn3a3PmxxwHQLazLtXgLtHulsnBD32nSqeuW1t60OLgLsStx1a7tMRhxvWUiROxcGweAkvww)](https://www.udacity.com/course/viewer#!/c-nd000/l-4195258602/e-48538418/m-48733149)

**  
**

**Order by Clause**

![](https://lh4.googleusercontent.com/YyXgN0IZaYooehjH3eFkLJ935AaYzhp7wCm2w1MjE1ziLzq6hin-6wfMsCsE1ZhiJ_mKq4no9-2Me433Xl2FsveGopZgOdcdPB19Zatsn23y64epiK25jlRoyj_H7DBVYH3IUSO8)

* **It says to sort the results\(排序\)**

* **說明**

* **原本的排序是 ascending order**

* **ASC = ascending**

* **DESC = descending**

* **where clause is not required**

**  
**

**Join Query**

* **you can use that involves multiple tables**

* [**介紹**](https://www.udacity.com/course/viewer#!/c-nd000/l-4195258602/m-48673663)

* **另有隱情，為何我們會不常用？**

![](https://lh5.googleusercontent.com/r2w2Ei1AXiVY-wmiN6dgEFD3ffZ-_e0edPXqtEszpdMem4DYro7B7-JzrVruDNN7MjJm1Wu3_b_JJ1hAw4ePA0NOLabh9YVAdR25NPjReAIvi-r8hz0mw7GCaal91UXdw2I0oj8X)

**  
**

**Indexes**

* **不用用眼睛搜尋**

* **就像書的目錄**

* **增快 queries 的速度**

* **hashtable 就是一種例子**

* **python 中可用 dict 表示**

* [**介紹**](https://www.udacity.com/course/viewer#!/c-nd000/l-4195258602/m-48734223)

[![](https://lh4.googleusercontent.com/LPigPxmuxFsalJ0EUGP6CJKbw52y39BUtWFUc_gm8hl25vLCCKtxZ0NEmQEgfu-Vva31VQIMo2r0_k6MOC7-Yms1H-uFEpnYYbCJi7f_owVGJQpaOOlKHd7m2wJtHX2lWfdYjCcW)](https://www.udacity.com/course/viewer#!/c-nd000/l-4195258602/m-48734223)

[**輸入 link\_id 回傳 object**](https://www.udacity.com/course/viewer#!/c-nd000/l-4195258602/e-48538419/m-48727411)

[**輸入 link\_id，輸出變成 dict**](https://www.udacity.com/course/viewer#!/c-nd000/l-4195258602/e-48329858/m-48728234)

**利用這個 dict 直接去抓你想要的資料**

  
[**例子**](https://www.udacity.com/course/viewer#!/c-nd000/l-4195258602/e-48230542/m-48632779)

* **def link\_by\_id\(link\_id\):**

* **return link\_index\[link\_id\]**

**建議第二行使用 link\_index.get 這樣沒抓到資料會出現 none**

**  
**

[**創一個增加 link 的方程式**](https://www.udacity.com/course/viewer#!/c-nd000/l-4195258602/e-48230542/m-48739119)

[![](https://lh5.googleusercontent.com/JO0duRtc2jlHW6cyk2oY4C-4WDSpzrQpIhlZe2TdSVSt4PQQHUAtM9on2c5MJQN2jeViHchkEaXIC5v_6INM5ILuOIApDYMiWhTeey4rSB_fsGJM3G41twI5dwx5otU1SD6v-YGQ)](https://www.udacity.com/course/viewer#!/c-nd000/l-4195258602/e-48230542/m-48739119)

**第二點： When we're inserting new round or table, we also update the indexes, that takes time**

**  
**

**實際上**[**indexes 如何運用呢？**](https://www.udacity.com/course/viewer#!/c-nd000/l-4195258602/m-48682569)

* **count is a SQL command for counting the rows in a table**

* **explain analyze 語法**

* **explain what it did**

* **create an index id on the id field**

* **語法： create index hotel\_id on hotels\(id\);**

* **第一塊：name of our index**

* **第二塊：on 什麼 table,這個 case 是 hotel table**

* **第三塊括號內: which field we are going to use**

* **drop index hotel\_id;**

**  
**

**Indexed for sorting**

**  
**

**Hashtable**

* **沒有 sorting**

* **just a mapping key to values**

* **增加新 element ，新加入的位置沒有規律性，可能 positio\[0\]才是新的**

* **Looking up particular key , 檢查時間:constant time**



**  
**

**Tree**

* **Basic Data Structure**

* **Sorted**

* **缺點檢查比 hashtable 慢，檢查 function: logn，n 越大數量越大**

**  
**

[**案例： Reddit**](https://www.udacity.com/course/viewer#!/c-nd000/l-4195258602/m-48271895)

**  
**

**ACID**

* **transaction**

* **a group of statements, group multiple commands**

* [**觀念說明**](https://www.udacity.com/course/viewer#!/c-nd000/l-4195258602/m-48746017)**  
  **

[![](https://lh4.googleusercontent.com/gTU4ONruAXbcltruXk0lpfB0RS6RN1Y5vyY0N-dQHg2F6FcOQqT3esK7xBUHLfHUHkV0zyGjx6vOlub6gMP-enS6HsRJiZ9mF15VQPZAA6LkyXldxCCr_5YdfeX3Sq3oFKoAaamB)](https://www.udacity.com/course/viewer#!/c-nd000/l-4195258602/m-48746017)

**  
**

**Google app engine data store**

* **Instead of having a table for links, having a entity called link**

![](https://lh6.googleusercontent.com/4WA8Xzc7Zg-YaJu1saO0IQPbydOlE8WhBk4aAmFuSxMJpFyOBsELiK_ygiaWmScW9-eEKl0MhUTpLo02VU7aDiQVnh4krLBH5X2qwECAAK0elCHW8a77D8KGUeMhU8yriHWn42bL)

**GAE Entities**

* **The column are not fixed, google 表示 whatever column you want**

* **Table 是 fixed**

* **Same type 的 entity 不一定有 same column**

* **開發較簡單**

* **All have an ID**

* **entities have the notion of parents and ancestors**



