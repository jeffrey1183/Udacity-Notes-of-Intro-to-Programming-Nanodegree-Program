# **2.6 Structured Data:Lists & For loop**

### **Web Crawler**

**    
**

**介紹 List**

![](https://lh5.googleusercontent.com/6riPZN8K67I2O5tgPi2bmDnCf-sXiFjLbsTxEHdp5YBUkl8kz7KWP8235-KfSEWtfXrroj5MPcoOfkgEj9MgPtkdWZ4AEMoLJsAL8ZaCGvLo2FORSiCdiPAXmHt1Ky2pCGG-6KSZ)

**List 可以是String, Numbers, Characters或是另一個String**

**    
**

**Square Brackets 中括號**

**    
**

### **用法**

**    
**

![](https://lh6.googleusercontent.com/LpwTZmxyNze9WBv6xP7hX_WkCYWz_OkiShnnV_H0Zq1nlX00WM-_PYdmSGSPl8WeOAlOPzz9dDWCHj9B-BdZoBgTmu_bJUXtOfnfnXxT89xqY7fuI4grAeJvBkOw8nIneOb7Lx9H)

**    
**

**如果要讓顯示的數字顯示出 float，就在數字後面加上點**

**  
Lists of list**

**如何去抓 Lists 中的 List**

![](https://lh4.googleusercontent.com/XcDK_bqLxKwPJhftzKK4N4qzUf7fMmo8sHc8TrtnH-LOMKMX3mW5uMQNe7Inozd2PzVCvZkxYDYx5IKV1lcikmVuuHJaNeBV4jfYG_RnZYkiUxgVQ6t_JMPucVCwa8oGztYexlKm)

**    
**

### **Mutation**

**    
**

**Mutation （變種），改變列表的值**

**先複習基本概念，以下的例子說明：**

**一開始我們創造了字串Hello後，s的變數指向字串，後來創造出ＹＥＬＬＯ，Ｓ轉向他，最後再創造出ＹＥＬＬＯＷ，整個概念並非修改而是轉向**

![](https://lh4.googleusercontent.com/_eo_FK6wmLStIxOFXl2ixFbsvuVwPHI2CvNNIfyZVJVy3ukt_mQ35Jr_tezFnROfsHampqkFFLQ7p4DhPAvc7d2etR-W46HQE4i6VNXNbwvNJpt8l9s-PS2iF2J8L_2HJheSUO9D)

**  
Mutation最大的不同是：他沒有產生新的值，而是直接變換原本的值**

![](https://lh4.googleusercontent.com/MsjzHXXbb6mQhSrnf8cfhd44WOCpX2v_6QhumUX0pm4GBUYDjnEsswyeSJSPjPtFcKdG7Unb6qix26ex2N4zbqYpfCKMeHzfYXGTG6B2CErjrwVhh-tt4kjsnWKik83hYuIiwB2Q)

**    
**

**String中的值無法像ＬＩＳＴ這樣更改，但在ＬＩＳＴ可以，當兩個變數指向同一個值，改變其中一個substring，另一個也會變**

## **Aliasing 別名**

**指向同一個物件，牽一髮動全身**

![](https://lh5.googleusercontent.com/FeqVR4H9JgpfTW0949dVprFc2QdeD-by9w04hq4KBKfT_MXGGXY388Z-oqLbSGUpyFGGLzIkOVvl_kUikmg6twaCJgrArvO3SIg5hDZHmOFMW-5nwWVWId9NOWa31f5Vau170nCM)

### **List Operation**

**Plus**

![](https://lh5.googleusercontent.com/khnwd1KQLgiY0Xf2TK6GYsf8XHrjC6lIqv60Mhu92f4AzyXsoIwKskR8CX7VKk6Mb-jlpLAz0ztnpYnfr1dP6dVF8n8iOjqfegGhDRLmWxsHjCV-EseIpt97djqBrm2RPvWVamCH)

**Append**

**    
**

![](https://lh6.googleusercontent.com/rBvxbnSv2MufTPoakZ-xUHNZq4FyKCHrVyGIrvvPCU6glUP_9klC1LRIlOksGp7G8S-LYRIqfvJA_g4VgLTxsFH66ky3V5f2ZFR1II0iyQrf9Ish1K1rgWiE9XzJL3wPGVIyj4VV)

**    
**

**Length**

**    
**

![](https://lh5.googleusercontent.com/6lypCWNHloyB2PuqchWkQU2hvoAHtl7b0UET5fRJdX9JzN_FtrVc-GUzMlC_wFAEktRO8CTzkrtK2aDVlC9JT8w1qWKf9my2XP931WHXUZoLnPzcv1JYLodgjXlZ53L3A1fe5Z_w)

**Length 的題目**

![](https://lh3.googleusercontent.com/GHhxp_XXzNe8YB-Ejct9nTDe5srykZ4F4S2kHNAlvHqLFh0s5huvoPkg_rNhGbnXuHgX0XC68kxXP2gfx_VqJH7b_gAMsLlZOIAwHZt2o8NpflRkZY9bKCjTzsA1DR7GS32HELhb)

**  
For Loop**

**走遍列表的元素**

**對於列表中的每一個元素，我們將把元素指定給這個名字，然後執行程式塊**

**將按照次序走遍列表**

**使用 for 我們可以定義程序，比用while 的程式碼少**

**呼叫時傳入我們定義並儲存的變數**

**    
**

![](https://lh3.googleusercontent.com/y0uQ0ANZis2Uo7rLlS1jJz9zkhTIyvWs8cqP1sWWJRzowHP-3X1lORtBXIDwpO6-bjk5mpaY_tHQ10X9u4oAgZIY3c6JQIEVwHDAzaJGKZ-KlRGZTVGLC-SvCYT0FNsuDMTRN9Ji)

**  
Index**

![](https://lh5.googleusercontent.com/tU2fGDYVNJfQzSF2VOIenj3H-aZcwKH7BaU0o-7_aizVK066VEv8Eu-IowuIj1dkuRMo_NIzIlFr0HQKxinlKoi5aRFYm6TdT9OOhre2rM1LrzmSzOChs4vPwlpx6-7G5PEiIjCE)

**Value 代表著要找的值**

![](https://lh5.googleusercontent.com/HL34Myxz9R9amTgRMY7JdbRwumHbGehtzbkKgMlAsaJ5jqAv5GMM9gEtroZdxjVXsAT4Kx7qzLRXzDKngQTzi2MyDcdadv8D89mA7yJQZGxLLahRXogjRBzcWImSwz_0Rzi4929D)

**    
For**

**這是一個運算式，其計算結果是列表**

