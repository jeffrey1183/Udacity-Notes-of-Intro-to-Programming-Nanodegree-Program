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

## 為什麽我們將會看到一些HTML？

本課程主要在教 JavaScript，JavaScript 是讓網站“動”起來的語言，通常會用 JavaScript 操作網站的 HTML。在該課中，大家會通過使用 JavaScript 編寫 HTML 來生成一個網站。

HTML 的全稱是超文本標記語言。叫它超文本只是為了聽起來很酷，其實就是文本。

## Let's Start With Index.html

It describes the content and layout of elements on a web page.

* 在 head section 裡會找到一些 script links
* 在 body 裡會找到像
  * 文案, Hello World
  * div id = "main"
    * &lt;div&gt;s create empty boxes. 這個例子我們給他 Unique ID of main,之後 javascript 會用到

![](/assets/螢幕快照 2017-03-29 下午3.16.31.png)



### 現在程式架構上貌似有很多 sections，但填入履歷資料有哪些方式？

* 主要有 two obvious strategies ?



