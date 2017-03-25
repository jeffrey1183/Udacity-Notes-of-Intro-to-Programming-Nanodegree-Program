## 4.1: Front End Programmer

要處理像：

* Fast Loading speed

* Responsive Design

* 拿Design mockups 套 Java. HTML

  


### Front-End Projects

* jQuery library

* Video Games - Javascript

* Request to APIs

  


The goal for these lessons is familiarity with some important ideas in computer networking, the internet, and "server-side" programming.

  


![](https://lh4.googleusercontent.com/qufFYHbq_MvQJSRIw_X5kU58jW4TlYBiiANSSDmTZOoPtIHl4qxTlEkSt7LVS2IJm6vlB9C3f8qBy_TaHJFrkQi9N9eLtmA8PKn7Ovg8br883WMGKP8Xpj8gCYSTW_SYDO2SYXCf)

  


### API 完整解釋

  


#### 一般 API 都後端 build

Front-End Developers specifically make calls or requests to APIs but most often Back-End Programmers are the people who build these APIs.

  


#### API 經典文章

What is an API you ask? Read more about it in this[blog post](http://sproutsocial.com/insights/what-is-an-api/)

  


#### What Is an API?

API stands for application programming interface. As it’s a rather complicated concept, let’s break it down by looking at each of its parts.

拆成三個部分看

  


#### Application

If you have a smartphone, you are well acquainted with what applications are, i.e., the tools, games, social networks and other software that we use everyday.

  


#### Programming

Programming is how engineers create all the software that make our lives so much easier.

  


#### Interface

An interface is a common boundary shared by two applications or programs that allow both to communicate with one another.

So an API is essentially a way for programmers to communicate with a certain application

  


#### API: A Technical Perspective

further insights into the underpinnings（學說的理論，基礎） of this term.

  


“API is a precise specification written by providers of a service that programmers must follow when using that service,”

  


“It describes what functionality is available, how it must be used and what formats it will accept as input or return as output.



In recent years, the term API colloquially is used to describe both the specification and service itself,



例子 ”the Facebook Graph API.”

  


![](https://lh4.googleusercontent.com/TRxUmjX85vPGPb5zgO8mTjgWBMwxysMYUSpogdGqc0xR4EvZP-Wn4ND-iflN_arH_ciqIwi7DZM1W19YkGQD5Hcy1kMPw8FO1M8yXlIZ5RNfU3Bh5x8qC2udAyDyN60aJE1_KjLB)

  


#### API Analogy

  


Every time you want to access a set of data from an application, you have to call the API. But there is only a certain amount of data the application will let you access\(可能只有一些資料能取\), so you have to communicate to the operator in a very specific language—a language unique to each application.

  


#### 中間人的概念

To help visualize this concept, imagine an API as the middleman between a programmer and an application.

  


#### 取資料，怎麼問和怎麼接收

This middleman accepts requests and, if that request is allowed, returns the data. The middleman also informs programmers about everything they can request, exactly how to ask for it and how to receive it.

![](https://lh3.googleusercontent.com/C7nDnxlZCUKpMtqXRnpc6ma-gq-ukAko3KRaLNsitVsH1DGF2zrYWFin5MinHG0IMtSFmYAh0vD1HuuShWm6XKj2Lu5w2jpNbDyx9acN9HmCB7Dct-5CkUTZnkeZWCYj6-wrKFN7)

  


#### Example of an API

Sprout 去取 raw Twitter data，再生出介面呈現資料

we must pull that information from Twitter’s database.

  


![](https://lh4.googleusercontent.com/feLF9stxdg_-PlOLXdc427KPZhtDvsk91R2HEKkoSpZHMfBB-LpbNNYsR-PBZuIDp3nC5mTGGAFqAwKJXghC7PQCL9HNNZyU6o0V_tCH95GGrhRc-4sOVu2yjdl3sTpovQKEpZ6C)

  


我們不可能用寄郵件給 Twitter 或是不顧資安問題讓 Twitter 進入我們系統，所以That’s where the API comes in.

  


Our developers have written unique code that streams data from Twitter in real time so that whenever people request analytics from us, our platform is ready to package it all together nicely.

  


#### What Is an API Call \(其實就是用 request \)

Whenever a developer or tool requests information from an API, they need to call \(or, more technically speaking, create a request to\) that API.

  


#### 可能會有限制次數？

Many open APIs have strict limits on how many times people can make a call in order to limit traffic and not overwhelm the API with requests.

  


#### Why Are APIs Important for Business?

  


Do you use an application that tells you what the current traffic looks like? Or how about an app that shows when the next bus will be at your stop? Most tools like these rely on open APIs to run and pull the most accurate data. Those are both good examples of how open APIs might help you in your everyday life, but here’s how they can help you in business.

  


1. Businesses Create Apps With APIs \(就像 Mixerbox\)

There are many businesses out there that build software and tools that rely on pulling data from open APIs to help streamline a business process in some new way. In fact, without APIs, Sprout, as we know it, would cease to exist.

  


2. Business People Use Those Apps （讓世界更有效率）

APIs are important for business because they allow programmers to build amazing tools that help us do our jobs more effectively.

  


A good example is this[keyword tool](http://keywordtool.io/)that accesses Google’s search API to suggest keywords your business should target.

  


3. Businesses Rely on Open APIs（讓第三方開發者一同發展你的服務）

APIs are also important for the businesses that provide them, because third-party developers build out applications that further the use of the company’s core product. This saves the API provider both time and money. For example, before Reddit came out with its own mobile app, it relied on other tools created by companies looking to monetize that work.

  


### Learn to Use APIs

* [Codecademy 課程](https://www.codecademy.com/apis)

  


  


### 評估自己是否適合當前端

* [前端技術細項](http://blog.udacity.com/2015/03/web-dev-building-blocks-need-to-know-where-to-learn.html)

* * 我覺得內容是很豐富拉，但是實際去做比較實在。

* 大致可以分成兩種類型的前端

* Design focused developers create sites that look and feel intuitive to the user. They spend most of their time writing HTML and CSS.

* Application focused developers use frameworks to create logic that powers interesting interactions user experience on websites. These developers most often use JavaScript.

* 同理心 - 站在 user 的角度

* 拆解問題

* 與設計溝通

* Turn monolithic\(一大塊\) task into logical and reasonable chunks.

  


### What are important concepts Front-End programmers need to know:

* Focus on parts of the web that users see and interact with.

* Front-End developers access and present data from multiple sources on the internet through Application Program Interfaces \(APIs\).

* 多平台：A Front-End developer is someone who builds the interface on applications which run on a variety of devices. These interfaces should responsively transition from mobile to tablet to desktop.

* Every web page and web app is created with HTML, CSS, and JavaScript. All of the images, buttons, transitions, animations, drop-down menus, contact forms, and styling elements are all controllable using these technologies.

  


### 要學的技術 \(What are some Front-End Frameworks Front-End developers use? \)

* Applications are built on top of frameworks like Angular.js, Ember.js, Backbone.js, Knockout.js, React.js and Polymer.js. There are similarities and differences, however if you can pick up one, you can pick up all of them.

* Front-End developers use frameworks like Angular.js and Ember.js to organize data using industry-standard design patterns which help synchronize user actions and data with a web server.

  


  


### Javascript libraries like JQuery and to use CSS framworks like Bootstrap.

  


Java 和 Python 的比較

While Javascript and Python are different, they share similarities as well: functions, variables, data types, loops, and conditional statements find their way in both languages.

  


缺少影片說明

![](https://lh4.googleusercontent.com/oo9-WaUkJ04noyvc6pddaFq9hI6neYwCxvvjuqgImF0c8Q2igQqyfr8LCC8GUnbn1PQVVA6vT76nw0f91po4EM2OzpqxLUJvZi9t5kX_RIcocg-G9LxpTpTr3B2BFMqKU7mgM1st)

Java 要{} 和 分號， print 換成 console.log，兩邊的等號; city.visit

