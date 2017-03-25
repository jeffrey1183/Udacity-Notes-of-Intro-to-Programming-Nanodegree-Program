# **Stage 4-1 Instructions**

**Server Side 基本觀念**

* **A server is a computer that interacts with a request we make to the computer**

* **For example, whenever we type in "**[**http://www.google.com**](http://www.google.com/)**", we are sending a request to Google's servers to return a website.**

* **we can understand networks' effectiveness by measuring things like latency and bandwidth.**

**        
**

**Network**

* **Is a group of entities\(可以是個 organization 、團體、政府之類的\) that can communicate, even though they're not all directly connected.**

* **Messages go through hops**

* **最早的紀錄，written by**[**Homer**](https://www.udacity.com/course/viewer#!/c-nd000/l-4212668559/e-48011978/m-48688804)**，用狼煙通知戰情**

**每一個點都是 Nodes，第一件事是 Code messages，點亮訊息，we need a way to do routing ，了解路徑，了解經由哪個 nodes（截點）**

* [**Flooding the net**](https://www.udacity.com/course/viewer#!/c-nd000/l-4212668559/m-48729185)**像這個例子，整個都撒出去，也會有同時傳訊息的需求，我們要了解誰在用和傳什麼訊息**

* **        
  **

  ![](https://lh3.googleusercontent.com/sQOQxzGYeFORPvuFWQ-PcurpbCGL6KYFkCTkC6s4_qrEaff70_prFr_bUGRMfAeKJ4nrablL47Q97kXnWKFrqYE5TOAz07Rbn4BiM1cRAeW67Z9fjuTmCAJkqCQ7cIKns1L-fwcS)

  **        
  **

  [**Making a networks**](https://www.udacity.com/course/viewer#!/c-nd000/l-4212668559/m-48729185)

  * **Way of encode and interpret messages**

  * **一邊編碼，other end 解碼（interpret）**

  * **Way to route messages**

  * **Know the next place to send**

  * **Rules for deciding who gets to use resources**

  * **兩個訊息同時傳到同一個地方**

  **        
  **

  **Measuring Networks - 他們兩個很不一樣**

  **Latency**

  * **Time it takes message to get from source to destination**

  * **Measured in milliseconds**

  * **1000 milliseconds = 1 seconds**

  * **算開始時間和結束時間的差**

  * [**有什麼辦法可以增快**](https://www.udacity.com/course/viewer#!/c-nd000/l-4212668559/e-48737168/m-48729193)

  * **Making the signalling nodes further apart, it takes fewer hops**

  **Bandwidth**

  * **Amount of information that can transmitted per unit time**

  * **unit of information divide by unit of time**

  * **What's the rate you send information**

  * **Measured in Mbps**

  * **Mbps =**[**megabit**](https://en.wikipedia.org/wiki/Megabit)**per second or million bits per second**

  * **10的六次方**

  * **其實就是在看跑了多少0與1的資料**

    * [**Bandwidth Test**](http://www.cnet.com/internet-speed-test/)

    **Bit**

    * **Smallest unit of information**

    * **使用**[**箱子**](https://www.udacity.com/course/viewer#!/c-nd000/l-4212668559/e-48538415/m-48698551)**來比喻，0與1的概念，還提了用兩個問題就能問出箱子的顏色**

    **  
    **

    **Buckets of Bits**

    * **有多少種可能？**[**請看圖**](https://www.udacity.com/course/viewer#!/c-nd000/l-4212668559/m-48678760)

    * **2的 N 次方，每多一 bit 就多分一次**

    **  
    **

    **Protocol**

    * **Gives the rules about how a client\(web browser\) and a server talk**

    * **Client send messages in a particular way**

    * **Client sends a message GET &lt;object&gt;, server sends back a response - content of &lt;object&gt;**

    * **The protocol we use on the web is HTTP\(hypertext transfer protocol\), use to talk to server, then you request a document**



