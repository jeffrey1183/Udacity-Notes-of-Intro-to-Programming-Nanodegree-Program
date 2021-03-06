**4.7 HTML Templates**

**有趣的 tag:**[**marquee**](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/marquee)**跑馬燈 **

**  
**

**Hidden Inputs**

* **用戶看不到**

* **hardcoded value**

* **指的是 value="eggs" 這一段**

* **兩個 name 都設一樣**



**  
**

![](https://lh4.googleusercontent.com/SlnqHjVT5Rg40DGG_G6zpZky6E9VplCYAhE3Zvle76lDXTwzzUdaZCY1H5wMZ6acNDa1gwCU7kme6_YcGof64By11sCS78eYUcOEbj1TJpkcMHu3Fby8eL_KUt-BxjgXdwcqgIjV)

* **food=eggs，這一段可以叫做 hidden elements in the URL**

**  
**

**Shopping List Take One - 較麻煩**

[**說明**](https://www.udacity.com/course/viewer#!/c-nd000/l-4186408748/m-679078997)[**說明2**](https://www.udacity.com/course/viewer#!/c-nd000/l-4186408748/e-677309561/m-649059346)[**較好方法 - 用 Template**](https://www.udacity.com/course/viewer#!/c-nd000/l-4186408748/e-642099222/m-686819028)

**目標：創造 shopping\_list\_html 、hidden\_html、item\_html\(要塞到 shopping\_html 內的\)，把他們當作會遞增的元件，最終把元件遞加到整個要呈現的頁面**

**  
**

* **items = self.request.get\_all\("food"\)**

* **get\_all 會抓所有 get 和 post 的 parameter**

* **下方有**[**介紹**](https://www.udacity.com/course/viewer#!/c-nd000/l-4186408748/e-642099222/m-686819028)

* **下面建的 item 是 for 迴圈創造的變數**

* **item 用來替換 %s**

* **output 的值**

* **下半頁 ：output\_items 要加進 output\_shppping**

* **上半頁：output\_hidden 最後再加進去**

**  
**

**  
**

**Introducing Template**

* **A template library which to build complicated strings\(Web application 裡通常是 HTML\)**

* **這裡要介紹的 template library 是 jinja2**

* **原因**

* **運行在 google app engine**

* **東西多**

* **容易學**

* **輸入 HTML ，**[**會轉成語法**](https://www.udacity.com/course/viewer#!/c-nd000/l-4186408748/e-642099222/m-670849276)**\(**[**有避免的方法**](https://www.udacity.com/course/viewer#!/c-nd000/l-4186408748/m-668210172)**\)**

* **可以用 pipe escape\(\|escape\)**

* **或是在 jinja.env 加參數 autoescape = True**

* **\|safe 的**[**意義**](http://stackoverflow.com/questions/12341496/jinja-2-safe-keyword)

* [**http://jinja.pocoo.org/**](http://jinja.pocoo.org/)

* **yaml 裡要加 libraries 的 name 和 version**

* **import jinja2**



* 
* **template\_dir = os.path.join\(os.path.dirname\(\_\_file\_\_\), "templates"\)**

* **\# 連接兩個檔案**

* **jinja\_env = jinja2.Environment\(loader = jinja2.FileSystemLoader\(template\_dir\)\)**

* **\# 設定環境**

* 
* 
**  
**

![](https://lh4.googleusercontent.com/RL663HdOqYVF5nJXgvKQL_gfOjLXafoW65i7rGb08M9zXuarbwnC05LQ0pMuy9N5Y4FC_Tf8ccCB1KaD84lkXzyFCOjGLwnSV5QujDa6WKYUU4Z_7zFkvK4lMrKktkoGhKX_-wSP)

**Variable Substitution - jinja2**

[**\*a,\*\*kw 可變參數的用法**](http://stackoverflow.com/questions/3394835/args-and-kwargs)

* **這個**[**案例**](https://www.udacity.com/course/viewer#!/c-nd000/l-4186408748/e-668139084/m-647920898)**也有用到**

![](https://lh3.googleusercontent.com/04R540rRewnsGeEUhPqjdUnlsi4JomavXz2c0inp_lVARrindhdpiaHBFdtrVQvCkwU-pcUoW6_JDqUvQ2x1UYkylmD5J-OYAR32aOLvax3iyLxuyZvqiyQ18BEFzBDgr2z0Svf2)

**name="steve" 除了影響有兩個米字的預留變數外，兩個藍色的框框也有影響**

**  
**

* **要注意 shopping\_template.html 放的位置，跟 code 裡的路徑（template\_dir）有關**

* [**說明**](https://www.udacity.com/course/viewer#!/c-nd000/l-4186408748/e-668139084/m-647920898)

* **語法{{ Name }}**

![](https://lh5.googleusercontent.com/hiBm7Dasc1xw5uHyWzqYXB1IEk4wtMon0SuYpx-NomhstG01-DAEhS7vIuwqWXRIQBUOb5VRO9TxLB2Jw6cUXlJoszCMcteFYRkcqSz_yXcjqimfjmlG1z0PWxwlM2rzXsswWLxB)

**最後使用 get, 會有 q parameter, 可以在 URL 輸入 ?name=jeffrey 測試**

**  
**

**Jinja2 語法 - 都是用在 HTML**

**把 python 的語法套到 HTML ，很神奇**

**Statement Syntax**[**說明**](https://www.udacity.com/course/viewer#!/c-nd000/l-4186408748/m-684438754)[**下有語法說明**](https://www.udacity.com/course/viewer#!/c-nd000/l-4186408748/e-642099222/m-686819028)

* **{% if n==1 %}**

**For Loop Syntax**[**說明**](https://www.udacity.com/course/viewer#!/c-nd000/l-4186408748/m-684438754)

* **x \*\* 2**

* **平方的寫法**

**  
**

**Template Inheritance -**[**說明**](https://www.udacity.com/course/viewer#!/c-nd000/l-4186408748/m-678329737)

**當版型一樣的時候，真的只能複製貼上？**

![](https://lh4.googleusercontent.com/cthPfD5QCJgHJqJdioPr-ngXKj-iP31rjiupvJdjEPpKYQBc1qIvZl-2wzsr9Oyzw6VvglCXcbaWRXRZ761vjuzbkeFWTi_hgDAua4PDGkEEsjNy5uDF1v-QaserGSE9kds6X69P)

**創建一個 base.html ，讓他繼承別的頁面**

**被繼承的頁面 {% extend **

**"**

**base.html**

**"**

**%}**

