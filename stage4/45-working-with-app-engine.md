# **4.5 Working with App Engine**

![](https://lh5.googleusercontent.com/gg5XQoeFQMwQfoUcypkiQ98ZbREFlpLDhFT3AXgWTm02Mnri71hE-k_5BZqQcdk-hS0lZZ-zd1sqKWaIGluGzr0hWLYTyCdiC4fKzMVpv6lNBIX9hRgY9ay-_pmmXbQgIfRZgULr)

**分成兩個部分**

**  
**

**URL Mapping Section**

[**handler 解釋**](http://stackoverflow.com/questions/195357/what-is-a-handler)

**app = webapp2.WSGIApplication\( \[\(' / ', MainPage\)\]\), debug=True\)**

* **黃色部分**

* **1個 URL 和 slash，就對應 MainPage**

* **Mainpage 是一個 handler**

**  
**

**Class Mainpage**

**Inherit 了 webapp2 和 RequestHandler**

* **function 括號後面\(self，最常用的 parameter for class methods\)**

* **Request Handler from**[**google**](https://cloud.google.com/appengine/docs/python/tools/webapp/requesthandlerclass)

* [**webapp2**](https://cloud.google.com/appengine/docs/python/tools/webapp2)

* **self.response**

* **第一句先設定個 Content Type header**

* **By default, the content type is text/html，這個 case 設定**[**text/plain**](http://bbs.csdn.net/topics/40383143)

* **第二句就是 string**

**  
**

**修改 main.py 的內容**

* [**教學**](https://www.udacity.com/course/viewer#!/c-nd000/l-4150259168/e-48741146/m-48744006)

* **檔案類型可能會影響結果**

* **default type 是 HTML**

**  
**

**修改 action 和 class**

* **上面改了 &lt;form action="/textform"&gt;**

* **下面的 URL Mapping Section ，也要增加**

![](https://lh5.googleusercontent.com/84u4OLAL7MF6hXGTc2Ep0FCOPQnks8-rsaYkJmHjkaqkiPGAkV68M8HFR3_nBdZ8wHGWpRoN9xtwgp5VoZnR3XT68J-BTEsCDEHvgxVkTDmcd2BoV9JAAIlObi2Sw0CLq3P9vg9L)

* **response 是 send back to client**

* **request 是 request came from the browser**

* **這裡是 self.request**

**  
**

![](https://lh5.googleusercontent.com/4Os-7bh1NIz1a0a1ZQU3bIbNA2BU4zYQeiBBwZNdqIMDcr3dX4faxlQQmNwoXWHvFzAotJuqHKD3U4QgPHYottwsZteOJz5FpgSN-BskjWGjCTMShE89I7ze2uBZpE1nmtQjmaX1)

**get\("q"\) 後面這個 \("q"\) 參數視情況改變**

**  
**

**HTTP Request 實例**

* [**影片**](https://www.udacity.com/course/viewer#!/c-nd000/l-4150259168/e-48754023/m-48712345)

* **Debugging 的好寫法，看你的 HTTP Request**

* **self.response.headers\["Content-Type"\] = "text/plain"**

* **self.response.out.write\(self.request\)**

**  
**

![](https://lh4.googleusercontent.com/R8X_lSQ5AdVtnRMtEomaYJSCZQ7jIkjxNgYnChohIa8PL9BokUDBehMiQtXbPiftB_nzkRprK073BKSulbuBlnqq-tT45BBaFxcddHbFIOGTYH2mQ56s6LxYVTIzaKaXOoSWidaZ)

* **第一行 request line ，q parameter，接下來有一堆 header**

* **第二行 - Accept**

* **What languages we are expecting to receive**

* **第三行 - Accept Charset**

* **what characters are ok**

* **第四行 - Accept Language**

* **語言，很容易理解**

* **第五、六行沒講**

* **第七行 - referer**

* **告訴 Server，request 從哪裡來**

* **正確 referrer 的拼法是有兩個 r，但在 HTTP Spec 拼錯了，就一直將錯就錯**

* **This refers to the URL that sent this request\(可以知道發送 request 的 URL\)**

**  
**

**Adding form "method" - add a new attribute to our form**

* [**影片**](https://www.udacity.com/course/viewer#!/c-nd000/l-4150259168/e-48741147/m-48738068)

* **form method="post"**

**你的 method 改成 post，但是你的 handler 裡的 method 還在 get，會造成 error**

* **如果你不指定form 的 method, default 就是 get**

* **q parameter isn't in the URL， 當使用 post method 的時候 q parameter去哪裡了？**

![](https://lh5.googleusercontent.com/tOxOoQcoNiXTPaciTEiNJtXr91Hpp0mjuq2PtRPcd9jfCth3yM3dR0KOjgMdyMcwGcPKRDCPFIzGiH2B-xNUregOcuLPD56q8O_aoNvS7sybKfnKVflURArHO1zXZoWPNxwjpoKr)

* **第一行變 post，因為我們把 method 改成 post**

* **有些 header 重複出現兩次**

* **the fact that we're not printing the actual request,we're printing the python representation of the request**

* **發現 q parameter 在下方**

* **空格會轉成加號**

**  
**

**GETs and POSTs 的差異**

* **GETs include parameter in URL**

* **POSTs include the data in the request body**

* [**影片說明**](https://www.udacity.com/course/viewer#!/c-nd000/l-4150259168/m-48712347)

[![](https://lh5.googleusercontent.com/x4UTDmIqd4AJPzgdRjljkZe3FFVuFoTEmlPoSVc_lDpLAJg8ES8Rsb04NFx7jkhun7IAtFuc1tp6fdb2ciAlQQgLg0HtoRaGx5ahEftWGwgIZWM0Myg8RIQn2GVUiQEFsEbLWMAI)](https://www.udacity.com/course/viewer#!/c-nd000/l-4150259168/m-48712347)

**差別：**

* **第一點 parameter 的位置，詳見上面說明**

* **第二點，功能不同**

**GET 用來 fetch documents**

* **POST 用來 updating the data**

* **第三點，數量限制**

* **GET 在 URL 內，頂多 2000字**

* **POST 在 Body 內，不限字數**

* **第四點，Cache**

* **GET 存，POST 要更新資料，幹嗎存舊東西\(industry standard 也是這樣規定\)**

* **第五點**

* **GET 不會改變 Server**

* **POST 原本就是用來 update server**

* **通常一般的連結都是 GET request**

* **做 post 你需要用 &lt;form method ="post"&gt;**

**  
**

**  
**

**get parameters 的觀念**

* **When we've been doing get requests and the parameters in the URL are called get parameters**

* **used to describe what document or what page you're looking for**

**post parameters 的觀念**

* **used for updating server**

* **有破壞性（destructive）**

**  
**

**Status Code**

* **405**

* **4開頭, error from browser side**



