# 4.6 Validation

Validation 解決安全性問題

* verifying on the server

* 收到我們預期收到的

* 如果有 hacker ，你可能會收到 trash

* 循序圖

* 當user POST 資料給 Server，接收到正確或錯誤資料，回應訊息或重丟資料

* [說明](https://www.udacity.com/course/viewer#!/c-nd000/l-4175328805/m-48724380)

[![](https://lh3.googleusercontent.com/vjRfajSTYz0POnHnxv9wa-CL-nJRDRE9h05OAEkw43dHjIbz8JsJFM5h10khuJqaldF6RoWUPhjo789SJfM7r3_11I2dSBtYte57RvlYS2xaBFKHABaKdC2xC62zX44I0bsMkbEk)](https://www.udacity.com/course/viewer#!/c-nd000/l-4175328805/m-48724380)

  


  


接下來的問題

* 安全性

* You don't yet know how to add forms safely

* 怎麼存 Data

* store the data that you get. Without this ability, users won't be able to modify your page.

  


第一個字大寫 - Python 語法

* string.capitalize\(word\)

  


After you learn about input validation, you'll learn how to use Python string substitution to generate complex strings from data.

  


檢查月輸入 - Python 語法

* 學習如何使用 dictionary

* [說明](https://www.udacity.com/course/viewer#!/c-nd000/l-4175328805/e-48754025/m-48635673)

* month\_abbvs = dict\(\(m\[:3\],m\) for m in months\)

* 用 GET function on a Python Dictionary

* [說明](https://www.udacity.com/course/viewer#!/c-nd000/l-4175328805/e-48754025/m-48635673)

def valid\_month\(month\)

* if month:

* short\_month = month\[:3\].lower\(\)

* return month\_abbvs.get\(short\_month\)

抓到的 Key 如果 mapping 就丟出 value

  


檢查日輸入 - Python 語法

* Everything we get from web or app 都是 strings

* HTTP 和 Web App 不知道使用者打的是 strings or numbers

* 所以使用 isdigit\(\)

* [說明](https://www.udacity.com/course/viewer#!/c-nd000/l-4175328805/e-48736181/m-48634787)

  


檢查年輸入 - Python 語法

* 跟日輸入一樣

  


[套用到檔案內](https://www.udacity.com/course/viewer#!/c-nd000/l-4175328805/m-48714318)

* Responding based on verification

  


String Substitution

tuple:變數值組

* Converts the value of objects to strings based on the formats specified and inserts them into another string.

* [說明](https://www.udacity.com/course/viewer#!/c-nd000/l-4175328805/e-48750078/m-48719293)

* 單一取代

* "%s" %a

* 用a取代s

* 多個取代

* "text%s text%s" %\(var1,var2\)

  


如果當我們想要重複使用 same string and same variable twice

避免有一堆 %s，你還要算有幾個

* "text%\(NAME\)s"text" % {"NAME":value}

* 前面用括號包，%s 變成 %\(Name\)s

* 後面用 dictionary

* name 可以用在 string 裡很多次，dict 內也可以有很多組

* [說明](https://www.udacity.com/course/viewer#!/c-nd000/l-4175328805/e-48740149/m-48204989)

* given\_string2 =

* "I'm %\(nickname\)s. My real name is %\(name\)s, but my friends call me %\(nickname\)s."

*   * def sub\_m\(name, nickname\):

  * return given\_string2 % {'name':name,'nickname':nickname}

  


  Substituting into our form

  檔案名：4.6-2 verification[解說](https://www.udacity.com/course/viewer#!/c-nd000/l-4175328805/m-48746044)

  目的：告訴 user there was an error

  ![](https://lh5.googleusercontent.com/Iv-D-x0Ve9w_YRtrsWDvLr_yObRc4-EvIvaxj9wgsyPCWg9Yg3Psqz2EDoNNqh0wjER4yQ1O1WalPbsvETW4fvk4WKH9HkrxFOTp3KzznJmPSrE7kSvqL2tTMKfchBBlFLYdShWI)

  * 利用剛剛學的，放一個 string substitution

  * 還可以補上 CSS

  * &lt;div style="color:red"&gt;%\(error\)s&lt;/div&gt;

  


  接著去寫一條 function 當有 error 的時候要用的

  ![](https://lh5.googleusercontent.com/wwZjs5wzZuC-8y1xklSBv5MwmBKQ3FoeWYt1NiaYk5ctOhmPReVyHJEn3C1qpMXmyh4LbmCsft0yqvoMagg2sfaYjFRG9y8GW_uH3wrSivqCli9RM05mBvPWwh94VJZsdzp8FnYV)

  * 用 optional parameter

  * response 是用 string substitution

  


  ![](https://lh5.googleusercontent.com/oPOz6uxNDjqYfqEwxrHF9MmeDSdrM1W0OR0nB1Lotqi23mlRtnHPs0YfkmqdBsMhaZPLYUpTyyWP-4kdJzdJ72sgoT-w9QGpsPjxe0UDCNot6yjAyzLhaCrdo21YM33PXw4vjhE_)

  * 整體來看

  * The string error in our form equals to the value of error\(最下方， dict 內白字\)

write\_form 的參數 error=""，也對應 the value of error\(dict 內白字\), it refers to error（紫色），起源於 form 內的 error

* 下面原本有用到 form 的地方，也可以套用剛寫的這隻write\_form function

* 因為 write\_form 內的 self.response.out.write\(form % {"error":error}\)，也有 draw form 的原始功能

  


Self 觀念

![](https://lh5.googleusercontent.com/TteqRDtQzLiZMWmj1vAz1kEJ7csQkOEHhvUbQ_hcQG0jGpXSJl9OOKkNAFma011Aij7l0t9LIPjA6W0ffXS8ikelssMn6621GoC-TdmSfJr609GLzu0j8lNsEXxaCbF4qxyV0BDj)

* 記得第一個 parameter 要填 self

* 不然你下面怎麼用 self

  


An Optional Parameters

![](https://lh3.googleusercontent.com/NqteM8S9QJyda5RIH8W0PEUUU0m1SFWYlVdAxr7Mz43PK5AJ7yFyTqnuHfhqNKf5F6fceUj1nl64f241vLrj32yTpph9Y5_fC2qmatiCcdXxqTEV6LoEUzBn0zmZn0ofRRPMEP5l)

* write\_form 這個方程式有兩個參數

* 其中一個 error=""

* 這就是一個 optional parameter

* 你可以指定一個值，沒指定就出現 default value 空字串

  


Preserving user Input - Input value

* &lt;input type="text"&gt;

* 加進 value

* 變成&lt;input type="text" value="cool"&gt;

* When we render the text box, 他就會有這個 default value

  


如何加進 string substitution 到上面的 text element case

* &lt;input type="month" value="%\(month\)s"&gt;

* 拿案例來演練和[說明](https://www.udacity.com/course/viewer#!/c-nd000/l-4175328805/e-48754026/m-48717294)

* 先把原先的 &lt;input&gt; 加進 attribute value

* 加進後下面的 function 也要調整

* 先把 write\_form function 加進這些變數\(optional parameters\)，同時你也要調整 form % {"error":error} 內的 substitution

* 下面的 post ，原本是判斷 valid，我們改成先去取 month,day,year 的輸入值，再去判斷

* 最後 if not 的判斷式有用 write\_form，write\_form 有增加參數，我們也要修改



![](https://lh3.googleusercontent.com/tGs9FJ8p7CS4NLGt-8EHg-urf_C9Mw0MbrzIMyjT-jbcqljOUHSgR8atit3zjZQvY8pr2hv2OZphr34ETDTkFk8hx6nHVP3zy980wH-D31dZ9RYwlgL-SLHIzszI2JoxLzuGuenk)

如果這邊的參數順序寫錯也會造成判斷的問題

  


Escaping - 避免輸入的值有 "&gt;

  


如果輸入的值中有引號\(quote\)

* 輸出會有亂碼

* 原因：Python string 不知道 form 內的格式是 HTML，所以我寫了"&gt;，他就取代了原本的 "&gt;，多出了一段，這一段多出的又顯示在畫面上

* [說明](https://www.udacity.com/course/viewer#!/c-nd000/l-4175328805/e-48754026/m-48700453)[更詳細的說明](https://www.udacity.com/course/viewer#!/c-nd000/l-4175328805/m-48634788)

* HTML 是允許 escape 或是改變這些輸入特殊符號的情況

* [說明](https://www.udacity.com/course/viewer#!/c-nd000/l-4175328805/e-48687830/m-48718335)

* instead of including 引號, we convert it to \(&quot;\)

* instead of including 大於\(&gt;\), we convert it to \(&gt;\)

* gt: greater than

* 小於\(&lt;\), we convert it to \(&lt;\)

* ampersand\(&\),we convert it to \(&amp;\)

* [案例](https://www.udacity.com/course/viewer#!/c-nd000/l-4175328805/e-48738174/m-48746045)

* 有兩個方法

* 第一個直接換：先換 ampersand，因為每個字換出來都有 &

* def escape\_html\(s\):

* for \(i,o\) in \(\("&","&amp;"\),

* \("&gt;","&gt;"\),

* \("&lt;","&lt;"\),

* \('"',"&quot;"\)\):

s = s.replace\(i,o\)

* return s

  


第二個方法：import cgi

* [解說](https://docs.python.org/2/library/cgi.html#cgi.escape)

* import cgi

* def escape\_html\(s\):

* return cgi.escape\(s,quote = True\)

一樣可以套用到 main.py

* 請見檔案：4.6.3birthday\_app

  


Redirect 的目的和做法

[解說](https://www.udacity.com/course/viewer#!/c-nd000/l-4175328805/m-48746046)

[![](https://lh4.googleusercontent.com/Sn4n5WDiTyZ6K4nXDn3AOFpz_a0hz14BKEI6JWpGTH1UPOi0UbwQrthZAfkFqWZC4n-TgL47uAM8qMDGpG0Nnl9wbeptrh88ZvpvthMOwiIFhqesBx_RqU-R3CS857FhckSCnB2k)](https://www.udacity.com/course/viewer#!/c-nd000/l-4175328805/m-48746046)

因為會遇到上面兩個問題，我們改了循序圖，導到其他頁

![](https://lh6.googleusercontent.com/tM34E54aVpWh3LNr7i4luCgmFmp-AFmNi1phG6tDxb5OMV32xfmXWPn5p3L8FwMD9MqpCaYL-tHmgkBnOGT0wvBt_vHk9fceuwV_QlmeM7elD5MnMRwNMOKCx7qMs3EJQpNz4am4)

  


目的

  
![](https://lh5.googleusercontent.com/JKDaWOELVkClUWJZmoriizVbL9KcMxfYjYMfZGjy7zzYt9NFgNC0AawQIwIEXRh6QybmsPD0Kyr5lVEECuLEfzPog6e9vWW0zeniwYs4mCFxC_dkID84h7VGps6qjS5CTW2JFldf)

第一點就生一個 class，去 def 內容

* class ThanksHandler\(webapp2.RequestHandler\):

* def get\(self\):

* self.response.out.write\("Thanks! That's a totally valid day!"\)

第二、三點：修改上面原本出現的錯誤訊息，直接導去頁面

* self.redirect\("/thanks"\)

* 同一個 domain 就只寫 path

* 最下面的 URL mapping section 也要改



