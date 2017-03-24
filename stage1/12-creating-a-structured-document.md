## 1.2 Creating a structured document

Website like a house.

HTML like the structure .

CSS is the decoration.

Javascipts are your interactive components.

![](https://lh3.googleusercontent.com/fwAzEjGKl6e1bMMsagpUoWRNiguKEpNJoMRpoNT1pd1k8WHKBLqUEat-Oz10N0zQqYrimjmVnoMX3p8Fk-djMuro0tNPqcj3f3m7L5lQTkF1eWahB8HCXZH5UVBpV7fj-25S7KSu)

### Logistics, Project 1, and Text Editors

* [Stage 1-Webcast](https://discussions.udacity.com/t/stage-1-webcasts/16000)第一篇

### Correctly nesting and closing tags

* 包 Tag 不要包錯，像下面這個是正確的

```html
<strong>
<a href="https://www.udacity.com">This site rocks!</a>
</strong>
```

* 不要忘記 Closing tag，像下面這個就忘記 &lt;/li&gt;

```html
<ol>
<li>Apples
<li>Bananas
<li>Mandarins
</ol>
```

### 工具 Correctly spelling tags

* [W3C Validator](https://validator.w3.org/)

### Chrome DevTools Overview

* [影片](https://www.udacity.com/course/viewer#!/c-nd000/l-4137489485/m-4274879923)

* 看[Transcript](https://discussions.udacity.com/t/stage-1-webcasts/16000/3?_ga=1.112159748.1464933134.1465252233)比較好，但內容其實只有講到基本的操作，像是可以在 Tool 上修改內容，下面我整理了一下。Transcript 加入書籤

**重點摘要**

* 可以直接在 Dev tool 更改看效果如何，反正不會存檔，要重來就 reload

* 安裝 Chrome 就可以使用

* 開啟 Dev tool 後可以在你有疑問的 element 按右鍵找到 scroll into view

* 會看到"Styles" 這一區，裡面就是 CSS Code

* [舊版網站](https://developer.chrome.com/devtools#dom-and-styles)[新版網站](https://developers.google.com/web/tools/chrome-devtools/)

* 提供的資料包含[DOM](https://developer.mozilla.org/zh-TW/docs/Web/API/Document_Object_Model)，還可以監看[後端](https://developers.google.com/web/tools/chrome-devtools/manage-data/local-storage?utm_source=dcc&utm_medium=redirect&utm_campaign=2016q3)的部分，可以看到[圖片讀取](https://developers.google.com/web/tools/chrome-devtools/network-performance/resource-loading?utm_source=dcc&utm_medium=redirect&utm_campaign=2016q3)的效能

### 分析結構 - Tree :[branching structure](http://assignments.udacity-extras.appspot.com/courses/html-css/samples/explore.html)

![](https://lh6.googleusercontent.com/MLTTe-6MrhVKJAIkAmcsnIJST8xUMEuyI_vap_p_ZUkk0BuuKOobF_-NH5JC5nyzkIcfUPd22tgk4U8bFdAUFSL4XAQaCyAXNzKhqENbvdpxzGyi1SH4uhiDcEMJooYlCAncsRWM)

[例子二](http://assignments.udacity-extras.appspot.com/courses/html-css/samples/style-2.html)

![](https://lh6.googleusercontent.com/AHCUQEO6rwMpD33kS5eJVxWC0M48trGb5_1hiPZlbH5pVbpHRpw8lW2-fpiAB5SSjBiqML7YxR0e9F2yDfAebKL7YstXHWV5gjRzQM6WF-quONh8849a391YYn1_qIdRt8Ko6tF-)![](https://lh6.googleusercontent.com/ZfKgdUtjdcQKXX0w5EKqYe0xkUTaCMOtS4BJxvjqccsMfNf1AqcAItItH0PFa84NXYOpTNdf9PYAkVBY7mUQeoyzQnZCBTXXD4cLd2vMMNPkNyxKQooaFDI0HiVgE6HlbLzk6Fue)

* HTML and CSS are both "languages"

* HTML controls the "structure" of a web page

* CSS controls the "style" of a page \(how it looks\).

* When programmers talk about the "DOM" \(Document Object Model\) they are talking about the tree-like structure of a page.

To learn more about what a "tree-like structure" means, read the first two paragraphs of the[wikipedia article on Tree Structures](http://en.wikipedia.org/wiki/Tree_structure).

### HTML- HyperText Markup Language - the standard markup language used to create web pages.

CSS- Cascading Style Sheets - style sheet language used for describing the look and formatting of a document written in a markup language.

DOM- Document Object Model - a cross-platform and language-independent convention for representing and interacting with objects in HTML \(and other markup languages\). The nodes of every document are organized in a tree structure, called the DOM tree.

![](https://lh5.googleusercontent.com/kBibDapqPQABrw9_k3SmFfuOAplw00exmSvyYLAeBxDmhJRjC_9yJ-SEDBfbcu655i0vp92iEhz6m3nWcZ_rnF-nFWTcic0J4tk8zrC7Jr_6r84XzG4DGW-Orr2hv8Hr3Rdr_VN9)

The browser turns HTML tags into elements that form a tree.

The document object model,or DOM, which is a standard convention for representing and interacting with elements in html.

## Boxfying

![](https://lh5.googleusercontent.com/B66BjREyFBn7MhBZIO71tcw5xdal9XV0_SOx9TZaS6HvY8q1Q7716DHC-MGniGv4rPEoYhZKm9IhTbAYgzPg-0GE9mPdJdCD__bnN5nfZ30_fYxTgj3n39E79hm_u9lZ8Ja-Ttio)

### 加上class attribute

![](https://lh5.googleusercontent.com/KLGuvrMaIxlQSIILYeXy3rGwytKbYjHX_B6uenl5am1Dq6WCtzCrVFV_I5YJlA4lZyMzMm53huQP5J6jS7QbeHIGW7vqUVOmQX3FSyktmnWSRJYWin6NnVoqx8jki9L1_9ue-Bef)



# Having to change 100 lines of code when you want to make the site look different.\(跟上面其實一樣\)

## 寫法 1：

```html
<div style="color : blue">this text would be blue</div>
```

## 寫法2,可以用style tags直接加css：

```html
<style>
div {color:blue}
</style>

<style>
  div {
    height : 50px;
    width : 50px;
    border-radius: 25px;
  }

.stop {

background-color: red;

}

.slow {

background-color: yellow;

}

.go {

background-color: green;

}

</style>
```

# Box Sizing and Positioning Summary

Flex Box Layout

```
.app {
    display: -webkit-flex;
    display: flex;
}
```

> [http://www.oxxostudio.tw/articles/201501/css-flexbox.html\]\(http://www.oxxostudio.tw/articles/201501/css-flexbox.html](http://www.oxxostudio.tw/articles/201501/css-flexbox.html]%28http://www.oxxostudio.tw/articles/201501/css-flexbox.html)

# 從實際案例學到的CSS

```css
.body {

    padding: 20px 10px;  /*前面指上下，後面指左右*/
    font-family: Comic Sans MS; /*字體都可以換*/
    max-width: 2000px;
    margin: 0 auto; /* The 0 refers to the top and bottom margins and the "auto"              automatically */
    font-size: 1.4em; /*字會變大*/
    text-align: center; /*字靠中間*/
    border-radius: 20px; /*背景如果是方形，可以造出角角*/
    color: white; /*當字體顏色用*/
    background-color: #294860;
}
```

## 補充em的介紹，再加上rem

> [http://jas9.blogspot.com/2011/09/pxemrem.html\]\(http://jas9.blogspot.com/2011/09/pxemrem.html](http://jas9.blogspot.com/2011/09/pxemrem.html]%28http://jas9.blogspot.com/2011/09/pxemrem.html)

```css
.lesson {
    background-color: #294860;
    border-radius: 20px;
    color: white;
    padding: 10px;
    margin: 10px auto;
}
```

## Padding 和 Margin

這裡的padding，可以讓裡面的字和背景空出距離，完全發揮padding的特性，margin的話就是整個divsion外圍的調整，有加就有差

小段落的上下行距調整

```
p {
    margin: 10px 0;
}
```

## list-style-type介紹

> [http://www.w3schools.com/cssref/pr\\_list-style-type.asp\]\(http://www.w3schools.com/cssref/pr\\_list-style-type.asp](http://www.w3schools.com/cssref/pr_list-style-type.asp]%28http://www.w3schools.com/cssref/pr_list-style-type.asp)

可以改變 list 的樣式，還蠻酷的

```
ul {
    list-style-type: none;
    /* this removes the bullets that show up by default in unordered lists */
}
```

[行高](http://www.w3schools.com/cssref/pr_dim_line-height.asp)

[找顏色的好所在](http://www.color-hex.com/color/dfeaf1)

[font-weight](http://www.w3schools.com/cssref/pr_font_weight.asp)

