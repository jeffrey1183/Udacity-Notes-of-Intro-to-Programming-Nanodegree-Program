**4.2 Make the internet work for you**

* **HTML Document Structure**

* **&lt;!DOCTYPE HTML&gt;其實有**[**很多種**](http://www.w3school.com.cn/tags/tag_doctype.asp)

* **Java script file和 CSS file 寫在 &lt;head&gt; 內**

* **這一節講 &lt;body&gt; 裡的 Content**

**  
**

**URLs**

* **Uniform Resource Locator**

* **有三個主要部分:protocol、host、path**

* **URL 裡定義了 protocol，但 protocol 不限於只有 http**

* **像這個**[**例子**](https://www.udacity.com/course/viewer#!/c-nd000/l-4169998949/e-48587890/m-48724341)

* **path 可能就只是一個 slash**

* **The minimum slash is a path.**

* **The document we want to fetch**

* **e.g. /foo**

* **Host**

* **A domain name or host name、IP address**

* **of the server has the document we want to access**

![](https://lh4.googleusercontent.com/SYJqzJbRwz8iqS2q1mpv1jJbSmwJqbStD2fD-ZG3CcKpsuDWboh5ud5mF3a4Rg11hHhAjIcyWg8HoiCY-OfqfOSnWP99U5PP6w5HcxVUBuHGu9trVb_ly7UmV6O20y9UGiiMycNw)

* **Fragment**

* **包含\#\(hash sign\) 之後**

* **用在 to reference a particular part of the page you are looking at**

* **當你看到 fragment 在 URL，it is not send to server when you make a request,it purely exist in the browser \(client\)端**

* **The fragment follows the query parameters, it comes last**

* **如下圖第二個例子**

**  
  
**

![](https://lh5.googleusercontent.com/2hc5_iN2GD9OOEjStqtW4Npk3fC-cA7hgoejbNpF1mrwfpBXBeMLT03jgLSNHqwDBayQ7ZZ9JJrPODkO1Cw3INkTneDtUuZY34nOJ4LGTQutNl67zROa5Msy--bXuO3OoGpzaREL)

* **port**

* **When you make a request to server,一部分是host\(the name of the machine or the location of the machine you're requesting \)**

* **為了要連上網路，你需要**

* **the address of the machine which is represented by the host**

* **port**

* **default 是 80**

* **如果要改要用 colon 加上port**

**  
**

[**實際練習**](https://www.udacity.com/course/viewer#!/c-nd000/l-4169998949/e-48587891/m-48439398)

**  
**

**  
**

[**IP address**](https://en.wikipedia.org/wiki/IP_address)

* **Internet Protocol address**

* **A numerical label assigned to each device \(e.g., computer, printer\)**

**  
**

**An IP address serves two principal functions**

* **host or network interface identification and location addressing**

* **The URL is the human readable locator which resolves to a numerical IP Address and represents, as Steve says, "the location of the physical machine which has the document we want to fetch."**

* **An example IPv4 address looks like this: 172.16.254.1**

* **A name indicates what we seek.**

* **An address indicates where it is.**

* **A route indicates how to get there.**

**  
**

**Query Parameter\(Get parameter\)**

* **有些符號不適合在 URL 裡使用，**[**影片**](https://www.udacity.com/course/viewer#!/c-nd000/l-4169998949/e-48011977/m-48311782)**中就提到問號**

* [**文章**](https://perishablepress.com/stop-using-unsafe-characters-in-urls/)

* [**foo and bar 的由來**](http://whatis.techtarget.com/definition/FUBAR)**（FUBAR）**[**解釋2**](http://programmers.stackexchange.com/questions/69788/what-is-the-history-of-the-use-of-foo-and-bar-in-source-code-examples)

* **e.g. ?p=foo&q=neat**

* **Name = value**

* **When you make request, 這是 extra information the server gets**

* **it affects caching 快取，整個改變了 URL**

**  
Cache簡介\(pronounced like cash\)**

* **something that stores data so that you don't have to retrieve it later**

* [**就像圖書館裡的書櫃，管理員先看看他的書櫃有沒有這本書，再去閱讀室找書**](http://computer.howstuffworks.com/cache1.htm)

**  
**

**Cookie**

* **指某些網站為了辨別使用者身分而儲存在用戶端（Client Side）上的資料（通常經過加密）**

* **HTTP Request**

* **Browser talk to web server**

* **HyperText transfer Protocol**

![](https://lh4.googleusercontent.com/kqfERxxuLZ7g9S1DMBYHfrC92p4N70BfEYGyzYw2g74JNbQirDCEn8sRwcfbUoXrt25myJV4cFhJPMh2MYu5ohZcah6aq-25QDti3LgkxU4Zh6AfV-r2nZn6L8cEb0Mvd6fz5wG0)

* **比方說現在要 request to web server 要開一個網址：www.example.com/foo**

* **這一串 www.example.com 是用來連上 host，if it is http, we are making a connection**

* **/foo 這一串 path 是用來 request**

* **他會先有 Request line，**

**  
**

**Request Line 有三個部分**

* **method**

* **什麼類型的 requests are making to the server**

* **最常用的是 GET, you GET the document from the server**

* **POST 也很常用，用來 sending data to the server**

* **path**

* **/foo**

* **documents we're requesting from the server**

* **包含/**

* **version**

* **結構是 HTTP 加上 / 加上 版本號\(version number\)**

* **e.g. HTTP/1.1**

* **大部分現在是1.1 版**

* **網址中的 host name 有在 the request line 嗎?**

* **沒有在裡面，request line 只有path**

* **the path is used for making the request**

* **fragment 不包含在 path \(\# 後的\)**

* [**例子**](https://www.udacity.com/course/viewer#!/c-nd000/l-4169998949/e-48756005/m-48299858)

**  
**

**Headers -**[**wiki資料**](https://en.wikipedia.org/wiki/List_of_HTTP_header_fields)

* **Request line is followed by a number of headers**

* **Fotmat**

* **Name:空格+value**

* **Name 裡面不能有空格**

* **value 什麼都可以**

* **你只要一 request ， request line 和 headers 都一起發送了，像Host 和 User-Agent 這兩個 header 比較常見**

* **網址已經有 Host 為何這裏還有 Host?**

* **因為一個 Web Server 可能會有很多網站，所以要在這裡寫**

* **User-agent 要寫 who is requesting, 可以知道what type of machine is making a request，如果網站被攻擊，可以用來做些rate limit 或溝通**

* **就像 Googlebot**

![](https://lh5.googleusercontent.com/3sBFd49GD7RlQ-ZHvpNXEDSoOi9cu9z_VW8x7Oct-3G-BHtVUKbw1WiEmuPkFBg533HZiU8GfeXf2-7Z8ANH0WoMsOcAixFvJdIqrf0fLqlbsCguUwKMtGu2Z8VtwTppmW7EjYnn)

**  
**

**  
**

**  
**

**Absolute vs Relative Paths**

* **在之前提到的例子，說下面一串的 path 是 /foo/logo.png?p=1**

* [**http://example.com/foo/logo.png?p=1\#tricky**](http://example.com/foo/logo.png?p=1#tricky)

* **但他沒說其實這是 Relative Path for the URL**

* **It gives an address that is "relative" to the host \(in this case, example.com\).**

**  
**

**  
**

**Response**

* **Server response that you requested**

**  
**

**Status Line**

* **相對於 Request Line**

* **Format**

* **Version of Status Line**

* **Status Code**

* **4開頭的問題可能在，browser side**

* **e.g. 要的檔案不存在**

* **5 is error on the server side**

* **Reason Phrase\(English description of the status code\)**

![](https://lh3.googleusercontent.com/ni0gHXAPD319tHdfuPY4OUtCB8EFVK1DBnFi-H236Fz_-n6-ua5hK0fnf12shqhRY0Zc20AqYUcZDhfaEzvDhW8Sr-3Z5J-Dw52wgRgy-m7fRSk9-diLkIP1rTkRFy9-qYpxu41f)

**  
**

**Headers - Status Line**

* **下面也是一些常用的，格式也是 Name: Value**

* **Server 這一項跟 User-Agent 呼應**

* **一般寫 The version number of server，但寫的太容易（vulnerability）可能會被 Hacker 攻擊**

* **Content type, type of the document being return，常用 text/html，如果是圖 image/png, image/gif**

* **length 並非必要,client 也會記**

**  
**

![](https://lh3.googleusercontent.com/orOGL7H_f2ADw5HO8U3gN3bMaH2Qy86hnQp9cUI4SXMhL9j078-VFDVhNz_r2mHXCMIftORMWxNWXvGP9tFOMZmZTBNfWuQsR7-43t2nU85OnsIFugjmoGiMZfTJYc1_9uDg00aW)

**Servers**

* **目標： Respond to HTTP request**

* **可以把 response 分成兩類：static 和 dynamic**

* **Static**

* **pre-written file，像 image**

* **90年代，資料都是靜態，只是把檔案放在 Server**

* **Dynamic**

* **on-the-fly\(運作中\) by a program that's running**

* **現在的網站幾乎都是 Dynamic, on-the-fly**



* **Web Application**

* **it lives on the web server**

* **it speaks HTTP and generate content that your browser requests**

* **All of those of pages in 各大網站 ,almost are built on the fly by programs called web application**



