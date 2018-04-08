看這邊要寫什麼前言可能要自己想，把下面的課拆成文章






# [What is HTML?](https://www.youtube.com/watch?time_continue=19&v=5Kjx-NOwcSc)
HTML is the heart of web. HTML is made of:
* text content(what you see)
* markup( what the content looks like)
* references to other documents
* links to other pages








## HTML Markup
HTML markup is make up of tags. The whole thing includes tags, we call element. It has opening tag and closing tag with slash.

![](https://lh4.googleusercontent.com/YZ-ITRT4SRrt3a8HuD5ehjWtvyy_VquhB91AWegwu3o0__Omr7lLLiSuVI6Rid-zWp1kK-zrEptsq922ebJcTleJe8-uxB0lYa1-boFcJhXmMwumkuzUtItzJsYDLIoeBdI4SoZu)













## Tag

* 在 [HTML formatting](http://www.w3schools.com/html/html_formatting.asp) 可以找到，許多常見 tag，例如
* `<b>` - Bold text
* `<strong>` - Important text
* `<i>` - Italic text
* `<em>` - Emphasized text
* `<mark>` - Marked text
* `<small>` - Small text
* `<del>` - Deleted text
* `<ins>` - Inserted text
* `<sub>` - Subscript text
* `<sup>` - Superscript text
![](https://lh5.googleusercontent.com/xohhu_Kaxq4tZZ9W4fL1_EFPDAhiroOuKsAeP_bEcAZziisBvmDWIyn2VJ7wVGypINmxI0Dp3kizszpZkdnOBKkAm6EWOJMd6FW2lSlG_EopyElEZUak8SygwRa73TNfAzTnF5Ph)

* 如果你忘記加 closing tag，在opening tag後的字都會變斜體。

## HTML Attribute
* 介紹 tag 的 attribute 與 value
![](https://lh4.googleusercontent.com/HLyxq0YzLcRhBQUag9gSPOHnE18h8O42slm_0YyRxlScsneqaNqCtZ6iM0pDt4gRbTNXdAy0aPaiOgR1uJyOhBE58cJowPaNAkdLRVFqohCmu0fxI0Me7I7HSZibAkDOxhTq8T-2)






## Images Tag
* 以 image tag 當例子，src 與 alt 是 attributes，url 跟 text 是 value。

![](https://lh4.googleusercontent.com/IWGJRWiA7gotFzri7C9Y40luRr_0GYQUXquMtnBha2UyTMTGcEzFhHG-Pf6ZENIIYTvafoQRn5YkarZ59EOXJ9S9fdiGKc_i3irvdEyFgeuRZLaXQ0zhpwSuyjINn_rvZWwuzin8)


* alt attribute
 * alt 的全稱是 alternate，當圖片連結失效的時候，就會顯示 alt 內的設定的字串。

* void tag 是指一個 tag 並沒有 content，他不需要一個 closing tag
* break 是換行的意思

##Whitespace
* 空格與換行的使用
 * 在 html 裡就算你空很多空格，但實際上只有一個
 *  `<p>` tag 的 p 是 paragraph, 段落的意思。


![](https://lh6.googleusercontent.com/iZt7H-X4pb4a3fqXKNZq0ytqAs_3jtuWoeUoOIuV_RAHnFjw8R8mqDg2y-xMPRHu8luKP-AhU5ZkCXSrHB5NxAT2UEfP1UzfVn161MazBaH0N2SxMiuPNUCiAGBIKYoLeNz_eRH-)

範例1

![](https://lh5.googleusercontent.com/B-DleTUXtOgLEi-EVz6pRwVSBwP31_CPhGDDDk-cQBp3JFfH9VPYq6kHN850Td8JX4Ati--t2h8fzQEAHHsH5tuW9Fg1-fRGT37g8ArZCax9j-fGzBZoTOOMjxQdxqKNJdvg8ZQ0)



## Inline/Block Element

* [官方解釋](https://www.w3schools.com/html/html_blocks.asp), creating "invisible boxes"


* block element 像 `<div>`、`<p>` 這些 tag。會創造有長和寬的空間，他會是一整塊跟畫面的寬度相同的空間，且從左開始。
* inline element 則不會是一整塊與畫面一樣寬的區塊，他的寬度會依照需要多少空間而不同。像 `<img>`、`<span>`。

![](https://lh4.googleusercontent.com/i4eEa_-2IJLg8hLGYsd67ET9uNpipgGzQdiOGW1bRXNpmu7O39RZ0zDQgyD_mUtfgTRkbYbtsLlSvb87LMkWYK40DqvgJTGZJ80mXvrDjWKXykAX2l3jyJq-gyNOF669im-ApeHD)

![](https://lh4.googleusercontent.com/vfLdVMUlhRavQ_fADnpV7wm_Wspj7DHGJduVoSNXdbMw9uxzMDQOcgRmeOLSVKFdHZn6Gc7grydM4FifTlEOLa6h14J91QoK4SjaLUm3f1DcZPQkeiwunT27ovDMxoKRNeLP4lhe)

### Quiz
* 哪些 elements 是 inline element?

![](https://lh4.googleusercontent.com/A2KSYadOLIuwIpk6x5OwSwGOTg9YzOmCMN8iWuLot-rDu1FhF0Twl3G17EOKGSN2EHgy3e3e_2UJt748BLy2zAf9tXsRAEwL6cS9ckhi1jrXVOKUb97vkg_LttjVzUdvm81KP-OA)

## HTML Documents
* doctype
* html, head, body
![](https://lh6.googleusercontent.com/I2vaef0mKXEvvQ0zerQYLPR7ZeSvpqJV5JHawxoFNkow9Cz5XPJh2U2okfpoofWCj3fg-ahalR9zLKjUDEc_UuOnrl9PTbYLH_lZ-Eu6chiUzhJTJRe8adj1oxFRNECb-rwdIKY3)


![](https://lh3.googleusercontent.com/m56kgVRSCArm0z9Z6NaO6rFDaKoeCCCHH72SVk_SAwYome1jMQzaEh51c3DTx-idKBSfifYoN0H-z57RuehLcv8UTJTy_CmJZd3yxWQvYu8i4ii4Al5BBoRctiXN65hCjgArodQA)

Review

First, recall the two main topics covered in this lesson.

1. Overview of the Internet: You were shown the big-picture view of how the internet works and were introduced to terms likeservers,browsers,the internet, andHTTP.

2. Introduction to HTML: You were introduced to HTML tags \(like&lt;b&gt;,&lt;p&gt;, and&lt;em&gt;\) and saw how even though these tags aren't visible to users of a web page, they still carry meaning thatismeaningful to web browsers.

## What to take away from this lesson.

The five most important things to take from this lesson are the following:

**1 - What a Web Page is**

A web page is a text document written in a language called HTML. Web browsers read these documents, and then interpret and display them.

**2 - How Coding Works**

Coding happens when programmers write text in a language that a computer can understand. The computer can then follow the instructions the programmer wrote. For example, the computer might do this by making text like this:

I'm &lt;b&gt;learning&lt;/b&gt; to code!

look like this:

```
I'm learning to code!
```

**3 - Computers are Stupid**

Programmers need to write exactly the way a computer understands \(also known as writing with correct "syntax"\).

For example, if you forget to close a&lt;b&gt;tag, the computer won't be able to figure out what you had intended to make bold. This "stupidity" can be very frustrating, but it also gives programmers incredible power: if you know how to talk to a computer than you can tell it to do anything you want.

**4 - Programmers Can't Remember Everything**

There are too many details to keep everything in your head. And that's okay. If you forget how to make text italic in HTML, you can always just look it up.

**5 - Basic HTML Vocabulary**

You will be using HTML in the next few lessons, so it will be helpful if you're comfortable with the jargon.

* Tag: An HTML tag is always contained within angled brackets. Most tags have an opening tag \(&lt;p&gt;for example\) and a closing tag, \(&lt;/p&gt;\). Some tags \(called "void" tags\) do not require a closing tag \(like the&lt;br&gt;tag\).

* Element: An HTML element refers to everything within a set of opening and closing tags.



**Attribute: **This is a property of an HTML element. For example, to set the href attribute of an anchor tag to the Udacity URL, you would write&lt;a href="www.udacity.com"&gt;




