# 5.1 Meet Javascript

* Using JavaScript to bring web pages to life.

* Using APIs to easily access powerful data.

* Two fascinating ideas in computing: recursion and parallel computing.

* How to solve big problems.

* How to make web pages look good.

  


這堂課

* To give you an introduction to JavaScript, which is the programming language of the web. \(基本介紹\)

* To serve as a quick refresher and review of important programming concepts like variables and data types. \(觀念複習\)

  


基本語法

* 建立變數

* var age = 32

* 不用擔心 integer 和 floating point numbers

* 因為都存 64 bit floating point

* 建立 array

* var myarray= \[\];

* 建立 function

* var function\(\){};

* 建立 object

* var object{};

  


  


紅綠燈的例子

* [案例](https://www.udacity.com/course/viewer#!/c-nd000/l-4128098911/m-4066358582)

  


Adding JavaScript to a Page

二個方法 -[說明](https://www.udacity.com/course/viewer#!/c-nd000/l-4128098911/m-4579894139)

* 直接加用 &lt;script&gt;

* 開.js 的檔案 \(較好\)

* &lt;script src="/path/to/script.js"&gt;&lt;/script&gt;

* 放在 HTML 的 &lt;head&gt; tag

  


To open up your browser console - JavaScript Console

* 把 script 寫進 HTML

* &lt;head&gt;

* &lt;script src="test.js"&gt;&lt;/script&gt;

* &lt;/head&gt;

* 瀏覽器預覽你的 HTML 檔案

* 按 command + option + J

* 檢查有沒有 load 成功

  


String.replace - Java

* var email = "abc@udacity.com";

* var newEmail = email.replace\("udacity","gmail"\)

* console.log\(email\);

* console.log\(newEmail\);



  


jQuery append\(\)

![](https://lh6.googleusercontent.com/Ppfv0pfMXQzpVHys73FmzhHSMlcXEr483zQGqQowiImjpsr6JoyGAZTLLWfWoEfq2lDfvoTQx4SPGnI6TCxkP0CEE2C1CgQk0xUPXT9cCXLLhc2fzcEvSgq6G5mTgplCV4v_AUuq)

* [jQuery Selector](http://www.w3schools.com/jquery/jquery_ref_selectors.asp)說明

* $\("main"\)

* main ID

Mixing replace\(\) 和 append\(\)

* [說明](https://www.udacity.com/course/viewer#!/c-nd000/l-4128098911/m-1916748790)

  


Prepend\(\) 和 append\(\)

* Adding something to the beginning of the HTML

* [案例](https://www.udacity.com/course/viewer#!/c-nd000/l-4128098911/e-1941688582/m-1932168585)

* 前者會把 code 加進 division 的頭，後者加到尾巴

* [解說](https://www.udacity.com/course/viewer#!/c-nd000/l-4128098911/e-1941688582/m-1929528625)

  


string.toUpperCase\(\) 和 string.slice\(\) method.

* [案例](https://www.udacity.com/course/viewer#!/c-nd000/l-4128098911/e-2885918558/m-2857248576)

* .slice\(start, \[end\]\) ，沒寫尾，就算到最後一個字

**  
**

**  
**

* 
**  
**

**  
**

![](https://lh5.googleusercontent.com/mpF-X0QeqQiWcSpzHZQ8YRu5JXs2vLELkugHLwb3-4T-H-ui5ucFQPfQFTnO3xU067amPzehGFdpEMm6IsHAW7KGAIth2x8UruAmOFuDOi44Urei3FvKoXSAHAtsF5oY2KQlB5UE)

**不是每件事都有絕對的 true 和 false ，所以產生了他們**

* **NaN = not a number**

* **Undefined: variable doesn't exist and the interpreter doesn't know what you're referring to**

* **Null: variable exists but no value\(usually used placeholder\)**

* [**小測驗**](https://www.udacity.com/course/viewer#!/c-nd000/l-4128098911/e-1936658586/m-2253748563)

[![](https://lh4.googleusercontent.com/7Tvtlkm09qomklRB4AeyIrjUSnr1dHDh8NibDJv-tttrpM3dLB8e9DZKn7q-gYQQmABpFP4Z9HfRd62YkZQnt5dxse763rfUoM4GuQ5WQFu4lDB4C-InfPtymkldeFS3iKSg2EuY)](https://www.udacity.com/course/viewer#!/c-nd000/l-4128098911/e-1936658586/m-2253748563)

**Array**

* **In Javascript just like list behave in python**

* **var myArray = \[item1,item2\]**

* **square bracket 方框**

* **Javascript arrays are zero index**

* **加 array**

* **$\("\#main"\).append\(skill\[0\]\);**

* **The length of an array is the number of items in it**

**  
**

[**pop\(\) 和 push\(\) 的應用**](https://www.udacity.com/course/viewer#!/c-nd000/l-4128098911/e-2864068546/m-2872888538)

[**大小寫的應用**](https://www.udacity.com/course/viewer#!/c-nd000/l-4128098911/e-2325218536/m-2316138537)

**  
**

**Objects**

* **There are no classes in Java , just objects**

* [**說明**](https://www.udacity.com/course/viewer#!/c-nd000/l-4128098911/m-1953578553)

**  
**

[![](https://lh6.googleusercontent.com/7a3CfROkfqBGjjVz7DhbQ0Xo8bhmPHR0z_IUVTpvFW5MV-jPrewLsp4ReXdcVo92G1cde2jGblpsZo7GLceYC8i8Oi5fc8G0_0hRd9wrKuQceTqfND6EKQtfbcfjYCToUo4OMddF)](https://www.udacity.com/course/viewer#!/c-nd000/l-4128098911/m-1953578553)

**Dot Notation**

* **上面的例子，可以用 bio.name 去抓 "James"**

* [**說明**](https://www.udacity.com/course/viewer#!/c-nd000/l-4128098911/m-1925408565)

* **還可以 define outside the curly brackets**

* **語法：myObject.property = somevalue**

* **不需要 var ，因為我們不是在創造變數，我們在 creating property for object**

**  
**

**Bracket Notation**

* **跟 Dot Notation 類似，**[**相關文章**](http://www.dev-archive.net/articles/js-dot-notation/)

* **語法：myObject\["property"\] = somevalue**

![](https://lh4.googleusercontent.com/c6d75snm6-SD_xyxvBhhaAfWLit1vVpXP6E9M95yYAPHq7l80CWTLTqLl9J5RLEuxB5Vzkx6Pp9KUgxAx110gRHK-pPHsAB73MrIAS3Zl_7JEZte85HuuJxA7D5bDQLhccO60Hqn)

**  
**

**JSON - JavaScript Object Notation（object literal notation）**

* **storing and transferring nested or hierarchal data**

* [**細節**](https://www.udacity.com/course/viewer#!/c-nd000/l-4128098911/m-3095768545)

* **Internet GET and POST requests frequently pass data in JSON format**

* **With a mix of nested curly braces, square brackets and commas, it's easy to make mistakes with JSON. And mistakes mean bugs.**

* **檢查你的**[**JSON Lint**](http://jsonlint.com/)**.**

![](https://lh6.googleusercontent.com/SA6h5UNn2BtOzQOxfchRtMyYksUHWeHnXc64GYGHqbQSiEvKhbyi2H0floa2m8xVQCsx9jZ2-Ao6Bv2HYg2HywAU0G1VIkM4PwIgJw7O4plsK4SVXGwK562bvlqjM4w89REe-Blt)

[**解說**](https://www.udacity.com/course/viewer#!/c-nd000/l-4128098911/e-1950678559/m-1936858588)

