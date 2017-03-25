3.2 Use Functions

  


要解決的可能有兩件事：

1.計算時間\(time.sleep\)

2.打開 Browser

先解決第二件，google 打開 browser 的[語法](https://www.udacity.com/course/viewer#!/c-nd000/l-4182338913/e-997789312/m-1037248562)\(Webbrowser.open\)

3.印出現在時間：print\("This is time"+time.ctime\(\)\)

* ctime 是 counttime的意思

4.可以用 ctrl+c 在 IDLE 暫停

  


介紹資源[Python Standard Library](https://docs.python.org/2/library/)

  


[改檔名的練習](https://www.udacity.com/course/viewer#!/c-nd000/l-4182338913/m-1015728608)

1. Get file names from folder -[Python](http://stackoverflow.com/questions/3207219/how-to-list-all-files-of-a-directory-in-python)

2. 使用 os.listdir \(r"C:\OOP\A"\), 意思是 operation system lists everything a directory，裡面的值要輸入路徑\(path\)，Windows 可以直接複製路徑，Mac 可以按右鍵開啟簡介查看路徑

3. 括號內的 r 是 rawpack，原始的意思

4. Rename each of file

5. 找出 module os 中用來 rename 的 function

6. dst 是 destination

  


### The string function translate

Documentation for string translate, you will see

* [string.translate](https://www.udacity.com/course/viewer#!/c-nd000/l-4182338913/m-1015728610)\(s, table\[, deletechars\]\)

* optional deletechars \(we know it's optional because it's in square brackets\)

* 括弧裡的不一定要有

* [table 資料表](https://msdn.microsoft.com/zh-tw/library/ms175010%28v=sql.120%29.aspx)的介紹

* 這裏沒有就填 None

* os.getcwd

* cwd:current working directory

* 找出現在的 directory 在哪

* os.chdir

* chdir:change directory



* [最後來客製化你的字串](https://www.udacity.com/course/viewer#!/c-nd000/l-4182338913/e-997789326/m-1015728619)

* 玄機是每一個檔名都包含數字和英文，這些英文雖然都是城市，但只要注意最後呈現會照 alphabetically

* 先想出你要呈現的字，排出來後，再自己加上數字打亂他（加上數字後整體會按照數字大小來排）



