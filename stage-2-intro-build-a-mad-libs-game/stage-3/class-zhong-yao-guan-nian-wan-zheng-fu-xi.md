Class 重要[觀念完整複習](https://www.udacity.com/course/viewer#!/c-nd000/l-4185678656/m-1013629072)

* class variables

* 就是在 class 新增一個變數，associated with class created

* 所有用這個 class 創造出來的 object 都可以用這個 class variables

* [課程說明](https://www.udacity.com/course/viewer#!/c-nd000/l-4195428894/m-1010748723)

[![](https://lh3.googleusercontent.com/vCLvcuuh1yQs73cH8wOMyK-UQURwdvI8LpzskUQY30eK9EuUxMZepb66QcQ5FrQayavmn6hlZXjFFF2shWGemPf9WLfr6y79eDbuvJEOFqRRbdvnAfuJflH0I6BWx79VUUwearsY)](https://www.udacity.com/course/viewer#!/c-nd000/l-4195428894/m-1010748723)

[How to use list or arrays in Python](https://docs.python.org/2/tutorial/introduction.html#lists)

Array vs List

* [http://sharecoder.blogspot.tw/2012/10/arraylist.html](http://sharecoder.blogspot.tw/2012/10/arraylist.html)

* Array 需要連續記憶體

* Array輪循速度比較快，List輪循速度比較慢

* Array無法新增或刪除其中的元素，List可以

* 99.9% of the time, you'll want to use lists. They're flexible, and good for pretty much every purpose.

* However, there is also an array.array class in Python, which is essentially a thin wrapper on top of C arrays.

* [http://www.wired.com/2011/08/python-notes-lists-vs-arrays/](http://www.wired.com/2011/08/python-notes-lists-vs-arrays/)

Predefined Class Variables

* [預先存好的一些變數](http://www2.lib.uchicago.edu/keith/courses/python/class/5/)

* 像 \_\_doc\_\_

* The function’s documentation string, orNone if unavailable

* 可以用 Triple-quotation marks，在定義 class 的 function 內

**\_\_name\_\_**

* **The function's name**

* **\_\_module\_\_**

* **The name of the function was defined in or none**

**        
**

**Triple-quotation marks**

* **Defining a documentation in multiple lines**

* **用這個就不需要用換行符號**

* **\# 是 python 的評論符號**

* [**案例**](https://www.udacity.com/course/viewer#!/c-nd000/l-4195428894/e-997660292/m-1023048585)

**        
**

**Inheritance**

* [**說明**](https://www.udacity.com/course/viewer#!/c-nd000/l-4195428894/e-997660294/m-1017019081)[**實際的程式邏輯怎麼跑**](https://www.udacity.com/course/viewer#!/c-nd000/l-4195428894/m-1018768599)[**案例**](https://www.udacity.com/course/viewer#!/c-nd000/l-4195428894/m-1017678709)

* **class Child\(Parent\):**

* **Parent.\_\_init\_\_\(a,b,c原有的\)**

**        
**

**Inheritance Method**

* **你同樣可以def 一個 method，Child一樣可以繼承**

* **Method Overriding - 但是如果你在Child class 內加了和 Parent 一樣的 method，他就跑 Child 內的 method**

* [**實際說明**](https://www.udacity.com/course/viewer#!/c-nd000/l-4195428894/m-1026769120)

**      **







