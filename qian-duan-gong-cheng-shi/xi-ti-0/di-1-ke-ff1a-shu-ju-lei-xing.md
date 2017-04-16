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

### 練習 1

1. 打開上一章節下載的簡歷專案檔案，在 resumeBuilder.js 裡加入下面的程式碼後儲存檔案

```js
var firstName = "Jeffrey";
var age = 29;
console.log(firstName);
```

1. 接著打開 index.html 打開 Console 就會看到你輸入的 firstName，如下圖

![](/assets/螢幕快照 2017-04-15 下午7.png)

### 練習 2

1. 儲存一個變數叫 awesomeThought
2. 然後把 awesomeThought 賦予 "I am {{name}} and I am awesome! "
3. console.log\(awesomeThought\)


# String.replace method

如同之前提到的我們會用 HTML Template 去建置我們的 resume，現在先來練習一個改換字串的 method，我先設定一個變數，這個變數
存入我的 email




```javascript
// [string].replace([old],[new])

var email ="jeffrey@udacity.com";
var newEmail = email.replace("udacity","gmail");

// 不要忘記檢查一下有沒有成功運行
console.log(email);
console.log(newEmail);
```

![](/assets/螢幕快照 2017-04-16 下午1.20.09.png)







