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


### String.replace method 練習1 - 替換字串 + 顯示於頁面

除了剛剛的替換字串外，我們結合上一篇的 append，把 funThoughts 加進 main 這個區塊，讓頁面顯示 funThoughts 儲存的內容。

```javascript
var awesomeThought = "I am Jeffrey Wang and I am awesome.!";
var funThoughts = awesomeThought.replace("awesome","fun");
$("#main").append(funThoughts);
```
* 如果沒有寫 console.log() 在 Javacript console 不會出現。

### Mixing .replace and .append()
* 現在我們會用 replace 之後
 *  We can replace placeholders in HTML with real data.
 *  After that, we just need to append HTML strings to start building our resume.

#### helper.js

圖的右邊就是 helper.js 的內容，裡面有很多專案會用到的 helper data，helper.js 會比 resumebuilder.js (在下方)還早出現，當我們在寫 resumebuilder.js 時，也會先讀取 helper.js 的所有 data。

我們在 helper.js 裡會看到 HTMLmobile、HTMLemail 這些變數，每一個都有 `%data%` (place holder)，這些 %data% 之後會被 actual data 取代。

![](/assets/螢幕快照 2017-04-18 上午8.09.07.png)

#### How to replace `%data%` 
* 跟之前替換字串一樣是用 replace method

##### 實際操作
我現在要把我的名字加到頁面上，一開始我要設一個變數儲存我的 HTML 資料
```javascript
var = formattedName = HTMLheaderName.replace("%data%", name);
$("#header").append(formattedName);

// name 看你是要填自己的名字或是任何名字
```
1:24

https://classroom.udacity.com/nanodegrees/nd000/parts/9e3f43e9-2105-410e-9091-c09379e64606/modules/05e362be-d7a5-4865-91f2-0ec2cd031720/lessons/2f3d65c7-510c-4dd6-95f3-4f77d51309bb/concepts/19167487900923




