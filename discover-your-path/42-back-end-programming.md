# Back-End Programming

Clients & Servers 的基本觀念

* [說明](https://www.udacity.com/course/viewer#!/c-nd000/l-6596019581/m-6603678031)

* Client \(你的裝置\)，log in 你的帳戶

* 在 Twitter 輸入文字按下推文，其實就在做 post request 的動作，跟 server 溝通，然後再傳回電腦，Client create content and data and posting it to Twitter's database, and server return it back to the browser

![](https://lh4.googleusercontent.com/kKubGPTwOrxjz-453o96tUgxXpJcdi1Kv_SERWIiymRHrWAmJL9o6uA9-Y23IEYKIdMX1mK1cNEhi423kKjWk_8fhDf-uLIE80pgrg2P7fnFGE2OVZus8OE6POmh7seookQmVuUl)

  


POST Data On Internet

以狀態列為例子

![](https://lh3.googleusercontent.com/vz9TXuWa0lxJgNDFIZYwvLGtmJAuHFSq-vWbzAiHqE4cjB1j-JVhigMzZTZmOSm8s9DWcbMbF3vGovGEnccUUZd5z8cNE_-0UtN-QSGqLF92f1eMD_muRxCq2bJYzY9p7RtIRygV)

  


  


GET

* 你看到的資料

* Create a get request, getting the data associated with my account and retrieve it to my browser

![](https://lh6.googleusercontent.com/vkIm_GYY0i6MfiNCuExisEQB-q0hxD38PKCvU2afTlQcvmfKonmLBx4LFUaOykSgrKM52_9xROTHhed0sZPWcv8WJ40w92PP5ds2qky2feX6o5uHTzcEJ72zIQRYxg-hkNFBlACl)

  


後端要擔心的

* 平台的轉移

* 記憶體

* security

* 會不會有瓶頸\(bottleneck\)

* log 問題

* poke out from outside \(適時的點醒\)

  


Back-End Fact Sheet

  


What are the different types of backend programmers?

* Back-end programmers are differentiated by the languages and technology stacks they use. Back-end programmers can be generalists or they can specialize in areas like devops/infrastructure, internal tooling, api design, and database administration.

  


What are essential Back-End programming skills?

* Software architecture- The ability to translate project requirements into technical specifications

* Software deployment- The ability to make a software program ready and available for public use on the web.

  


What are the differences and similarities of Back-End programming languages?

* 一樣有很多程式語言可以完成後端工作

* Different languages are typically associated with different stacks, although some components are interchangeable between stacks. For example Ruby is closely associated with the Rails framework and ActiveRecord Object Relational Mapping \(ORM\), while Python has several competing web frameworks and ORMs.

* [Ruby on Rails](https://en.wikipedia.org/wiki/Ruby_on_Rails)

* [ORM](http://searchwindevelopment.techtarget.com/definition/object-relational-mapping)[基本介紹](http://rails.ruby.tw/active_record_basics.html)

  


Why might a backend language be more suitable for certain projects?

* Languages differ in how quickly a programmer can produce a working product but ease of development generally comes at the cost of performance and maintainability.

* Languages like Java and[Go](https://zh.wikipedia.org/wiki/Go)are popular among large teams and large projects because they enforce code organization and structure.

* Java 和 Go 在大專案和大的 Team 內很受歡迎，因為比較有結構

* Languages like Python, Ruby and Javascript allow rapid development and easy prototyping but they don’t necessarily scale to heavy loads as easily. This implies cultural differences between the communities around different languages, and in the teams that use the different languages. Java in particular is used at larger enterprises. PHP tends to be seen in legacy applications.

  


What are the important concepts Back-End programmers need to know:

* The concept of a stack: The ‘stack’ refers to the combination of technologies a developer uses to implement a particular project.

* One of the first major stacks was the LAMP stack \(Linux, Apache, MySQL, and PHP\).

* Over time more stacks have emerged that use different components. For example nginx is a popular alternative to Apache for the webserver component of the stack. There are many SQL and nonSQL alternatives to MySQL in use today, and there are even more choices of programming language and framework. Today the stack might also include the frontend technologies used by an application.

* The concept of full stack: A programmer who is competent in everything from Front-End to Back-End programming including all elements of the stack.

  


  


![](https://lh6.googleusercontent.com/OOSlOYv0-Ou4t6GzsBj2elYcrFLrZb9E4-TntW1ajcxDJg5KT_oFipxmazzZg6N3AfzitUU-uYt1fwSjOqjqjSmdIsXXKXsOi9mmTQf-Z69Xnx49A2eGjnzqfSpupJbF2495Q72b)

* 跟前端的溝通：How to display this data

* Storing or treating data

* 跟 Mobile App: How do I store client data in my mobile app

* 跟 Data analysts: How can I build a usable structure for this data

  


Ruby 和 Python 的小差異

案例： Build class for database that can store images

[說明](https://www.udacity.com/course/viewer#!/c-nd000/l-6596019581/m-6596005897)

[![](https://lh5.googleusercontent.com/_XunKz-YuLP0MAQN5ucYdnGiLNFfRtZ0IxGIoOslM_W4g8RivHGK2Bkeqsr7z1w2UTLRG-Uzm7BeZ_8RGlwtuCi6ia6liYmp5BxNf6QHE8hY_DoP8m0gF7Jad91S5ZQEeaqlX0DW)](https://www.udacity.com/course/viewer#!/c-nd000/l-6596019581/m-6596005897)

