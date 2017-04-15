# 資料類型 & 宣告變數 \(Variables and Simple Data\)

Javascript 如何用變數來存數據。

### Syntax

```
var {{variableName}}={{someValue}};
var myArray = [];
var myFunc = function(){};
var myObject = {};
```

* 我們會用 var 去宣告新的變數，不管是哪種 data type，即使是 objects

### 例子

```js
var firstname = "Wang"; // 字串加上括號
var age = 29;
```

* Javascript 與 Python 存數字的方式很接近，所有數字都是用 64 bit floating point，都不用為使用 \(float\) 或是 整數\(int\)擔心

### 實例

1. 打開上一章節下載的簡歷專案檔案，在 resumeBuilder.js 裡加入下面的程式碼後儲存檔案

```js
var firstName = "Jeffrey";
var age = 29;
console.log(firstName);
```

   2. 接著打開 index.html 打開 Console 就會看到你輸入的 firstName，如下圖

![](/assets/螢幕快照 2017-04-15 下午7.50.02.png)



