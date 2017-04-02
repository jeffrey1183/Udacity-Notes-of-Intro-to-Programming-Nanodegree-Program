# 簡歷專案\(Resume Project\)

---

### 專案目標

建置一個漂亮且有互動性的簡歷，放到網路世界上分享。你將使用 Javascript 逐步完成整個專案。

### 使用 Github 下載所需文件

1. 我們會使用 Github 下載需要的文件，同時在工作完成後，把簡歷上傳到 Github，沒有帳號的人需要註冊一個免費帳號。

有了免費帳號後，就可以來進行下面的步驟：

* 打開 Repository：[https://github.com/udacity/frontend-nanodegree-resume](https://github.com/udacity/frontend-nanodegree-resume)
* 點擊 Download ZIP

  ![](/assets/螢幕快照 2017-03-27 下午11.41.18.png)

* 把下載的檔案解壓縮，會看到這些檔案

  * **index.html**: The HTML file that will display your project. Open this file in the browser to see your work.

  * **css/style.css**: The styles for your resumer page.

  * **js/helper.js**: A JavaScript file with some helpful functions for your project. You won't have to modify this file until Problem Set 3

  * **js/jQuery.js**: A JavaScript library file that enables jQuery \(接下來會學到\)

  * **js/resumerBuilder.js**: This is where you'll do most of your coding for this project. It's initially empty but you'll soon fill it with lots of cool code!

本課程主要在教 JavaScript，JavaScript 是讓網站“動”起來的語言，通常會用 JavaScript 操作網站的 HTML。在該課中，大家會通過使用 JavaScript 編寫 HTML 來生成一個網站。

HTML 的全稱是超文本標記語言。叫它超文本只是為了聽起來很酷，其實就是文本。

## 簡歷專案 - Index.html

It describes the content and layout of elements on a web page.

* 在 head section 裡會找到一些 script links
* 在 body 裡會找到像
  * 文案, Hello World
  * div id = "main"
    * &lt;div&gt;s create empty boxes. 這個例子我們給他 Unique ID of main,之後 javascript 會用到

![](/assets/螢幕快照 2017-03-29 下午3.16.31.png)

### 現在程式架構上貌似有很多 sections，但填入履歷資料有哪些方式？

* Web developers 主要有兩種策略
* 右邊是 hardcode，就是寫死;左邊是用 HTML Template，fill it with data programmatically when user requests a page.
* 以這個案例中的 Work Experience 為例
  * 右邊就有一堆寫死的資料，左邊就還是 Empty
  * 右邊適合初學，但長期下來不是好方法，因為每次修改都要開 HTML 修改 
* 這個專案我們會用左邊的方法。
  * The browser will render this page just saying, Hello World.

![](/assets/螢幕快照 2017-03-31 下午1.32.17.png)

### Script Tag

在 Header 裡我們會看到下面 2個 script tag，在備註中都寫了 tag 的作用

```html
<script src="js/jQuery.js"></script> // link to jQuery library
<script src="js/helper.js"></script> // which contains some simple helper Javascript we've prepared for the project
```

下方還有1個 script tag

```html
<script src="js/resumeBuilder.js"></script> // Tell the browser to download and execute some javascript
```

* We will use the script to add HTML content to the main section of the HTML

### Overview of the index.html

![](/assets/螢幕快照 2017-04-01 下午5.44.41.png)

* 上面是 Hello World
* 中間是 Empty resume sections
* 下面是 JS
* 右邊是 how it would look in browser
  * resumeBuilder.js 會去撈資料，改變頁面的內容，目前設定了一個判斷

```js
if(resume.content ===""){
hide.resume();
}
```

## 簡歷專案的 CSS 跟 JS

* CSS 檔案存在 style.css 中，用來定義頁面風格，這門課不會學到 CSS，想了解更多可以看[學習資料](/qian-duan-gong-cheng-shi/xue-xi-zi-yuan.md)
* jQuery 是一個強大且主流的 javascript library，這門課會講到基本概念和初階的 functions，這門課的 jQuery 就算用 javascript 也能做，但是**主要是希望能增加使用 third party library 的經驗**。
  * It lets us inspect and manipulate the elements in a page.

## 練習: 使用瀏覽器的 Console

* We will use two tools, text editor to code and a browser to inspect our work.
* 現在的瀏覽器內建一套強大的工具，通常稱作 developer tools. 

### Developer Tools 簡介

* 讓開發者檢視網站載入跟運行。
* Dev tools 還有一個 Console，用來查看 Javascript 對網站的作用。

### 實際練習 - 在瀏覽器使用 Console

1. 打開 Chrome 
2. 右鍵按下檢查 或 Cmd+Opt+J\(Mac\)
3. 然後在 Console 裡打 console.log\("Hello world"\);
4. 顯示 Hello world

![](/assets/螢幕快照 2017-04-02 下午2.59.48.png)_**Console.log is basic print command for javascript.**_

* 不要忘記句尾的分號，雖然大部分的 javascript interpreter 都很聰明，知道那邊需要分號，讓程式一樣可以運行。

_**Console.log 就像 python 的 print command 可以用在 debug。**_

* Python 不用加分號

_**Undefined 代表沒有回傳值，告訴我們 console.log 沒有創造需要儲存 new data**_

![](/assets/螢幕快照 2017-04-02 下午3.13.00.png)

如果我們用其他 command 像 document.URL 就會得到這個頁面的 URL 的字串，就不會顯示 undefined

### 不同 browser 打開 Javascript Console 的方式稍微不同：

* Chrome：轉到查看 \(View\) &gt; 開發者 \(Developer\) &gt; JavaScript 控制台 \(JavaScript Console\) \([指南](https://developer.chrome.com/devtools/docs/console)\)
* FireFox：轉到工具 \(Tools\) &gt; Web 開發者 \(Web Developer\) &gt; Web 控制台 \(Web Console\) \([指南](https://developer.mozilla.org/en-US/docs/Tools/Browser_Console)\)
* IE 11：轉到工具 \(Tools\) &gt; 開發者工具 \(Developer Tools\) &gt; 控制台 \(Console\) 圖標 \([指南](http://msdn.microsoft.com/en-us/library/ie/bg182326%28v=vs.85%29.aspx#The_Console_tool__CTRL___2_)\)
* Safari：打開菜單欄中的開發 \(Develop\) 菜單： 首選項 \(Preferences\) &gt; 高級 \(Advanced\) &gt; 顯示開發 \(Show Develop\) 菜單。轉到開發 \(Develop\) &gt; 顯示 Web Inspector \(Show Web Inspector\) \([指南](https://developer.apple.com/library/mac/documentation/AppleApplications/Conceptual/Safari_Developer_Guide/GettingStarted/GettingStarted.html)\)



### Hacking Udacity - 用 Console 操控網站

1. 開啟新頁面，進入 udacity,com
2. 打開 Console
3. 跑下面這條 Command

```
$(".super-header-wrapper").html("<img style='width:100%' src='http://goo.gl/WCrBmS'>");
```

* Don't worry if you aren't familiar with CSS classes. The main point here is that`.super-header-wrapper`

  is an element on the page that contains the background and the jQuery method`.html()`changes what's inside it.

* 但是 Udacity 的首頁一直在更新，原本這條 command 是要換首頁的圖



