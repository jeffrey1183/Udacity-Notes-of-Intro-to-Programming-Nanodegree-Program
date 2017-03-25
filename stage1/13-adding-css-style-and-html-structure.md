# 1.3 Adding CSS style and HTML structure 

![](https://lh5.googleusercontent.com/OpwkWaAJQqGC9L9HXUIbI8koQ5ZoNcnPPtapYYoHyBxbJIRkK_4LTwNtsm2Yqq0f5IytSR3FeSqHS9rUU0v-X2fSL2vEom5ICLVb8syW4bjGbWsdTPKii_eIvFyFKSyNY8ZXFg6F)

  


### CSS Summary and Reference

內容摘要

1. 複習 selector,property,value 的觀念

2. 1. 跟 HTML 的 Element,attribute 用的名稱不太一樣
3. [HTML element](http://www.w3schools.com/html/html_elements.asp)是指有 opening tag 和 closing tag ，中間有 content

4. [HTML attribute](http://www.w3schools.com/html/html_attributes.asp)說明

5. HTML elementscan haveattributes;Attributesprovide additional information about anelement;Attributesare always specified in the starttag

  


### How do I include CSS Styling in my web page?

### 有三個方法



1.在head 裡面加一個style element，內寫CSS

2.用link tag連結你的CSS，&lt;link rel="stylesheet" href="main.css"&gt;

3.較糟糕的方法，Write your style inline with your HTML



### Code Comments

* In HTML, code comments begin with&lt;!--and end with--&gt;. Everything in between is ignored.

* In CSS, code comments begin with/\*and end with\*/.

### The Box Model\(邊框的概念\)

The padding is around the content, it’s affected by the back-ground color of the box. The border is inherited from the color property of the box.Margin doesn’t have the background color and it’s completely transparent.

The size of your actual element is equal to the sum of the border ,padding ,content width![](https://lh6.googleusercontent.com/GHjw5MDgUlvVnxYveWEf63A1jzqu3NOqV7pnc6o1BNt1RtzfpAjNkNastElGwsfYCI5zMU0jpgKnmKBiv4fDjJXYwC5ilaG2FcqaZ8_3c_PYSlGMyyXqxcs9SAZkHOf-tap2eGWg)

  
Total actual element width = 10+30+200+30+10 = 280pixels

  


## Box sizing

[http://zh-tw.learnlayout.com/box-sizing.html](http://zh-tw.learnlayout.com/box-sizing.html)

補充教材解釋了實際的用法，加上 box-sizing 的 property，設定 border-box，可以讓padding和border的增加，不會算進整個box的寬

```css
* {
-webkit-box-sizing: border-box;
-moz-box-sizing: border-box;
-ms-box-sizing: border-box;
box-sizing: border-box;
}
```

This calculation includes both the border , margin and padding.



## Box Sizing and Positioning Summary

Alt attribute:alternate information to the screen 讀不到的時候用來替代的

##  建置頁面的流程

![](https://lh3.googleusercontent.com/Dn4RZEP2SG9wl7Y35TCV3Xuu8H6GkwvpT92A2j6uuXVNuGAzQjVb1Vzp9GMLRe-62BhwNUtI29VeefC4k1U3gzgtPP5cdt_4qwVFojYkdF-PEg-XmoMqi4qRcXEDZ2wHVJdDFMEa)

  
  


