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



> http://www.oxxostudio.tw/articles/201501/css-flexbox.html\]\(http://www.oxxostudio.tw/articles/201501/css-flexbox.html



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



> http://jas9.blogspot.com/2011/09/pxemrem.html\]\(http://jas9.blogspot.com/2011/09/pxemrem.html

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





##  list-style-type介紹



> http://www.w3schools.com/cssref/pr\\\_list-style-type.asp\]\(http://www.w3schools.com/cssref/pr\\_list-style-type.asp



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





