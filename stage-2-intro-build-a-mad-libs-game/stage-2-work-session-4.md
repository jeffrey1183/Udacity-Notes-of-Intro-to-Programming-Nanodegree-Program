## **Stage 2 Work Session 4**

### **Random Nouns**

**What is randint function**

**  
**

**  
**

![](https://lh6.googleusercontent.com/SAOMRR_KJ45P5YBQnR6nwcpxegxFR88_ayoowwA4x2inUjsPp1LbofplrkcGjBVxWeQ42EuxwV35UqSGmOPnaWSkREzWE2ki_5RW-3Z_EA9IWpd-yCFuZeBnJX8z7UPMqJoUtxJw)

**  
**

### **Process Mad Lib: Solution**

[**https://www.udacity.com/course/viewer\#!/c-nd000/l-4196568648/e-4602638541/m-4945058538**](https://www.udacity.com/course/viewer#!/c-nd000/l-4196568648/e-4602638541/m-4945058538)

**  
**

**  
**

## **Stage 2 Submit - 猜字遊戲**

### **需求**

* **至少三關**

* **用戶一進去可以選難度，easy/medium/hard**

* **每關至少四個空格**

* **先顯示出題目**

* **quiz = choose\_quiz\(user\_prompt\)**

* **跳出輸入框**

* **確認要使用的答案**

  * **要選哪一組答案**

  * **loop**

  * **檢查答案**

  * **對會有 Corret**

  * **要把問題字串 spit 拆解，套入 replacement**

  * **return 出來**

  * **猜錯會有 Incorrect ，就要輸入 raw\_input 再猜**

  * **整段加上猜對的字要顯示出**

  * **global variable 的概念沒想清楚**

  * [**解釋**](http://www.python-course.eu/python3_global_vs_local_variables.php)

  * **一般在其他語言 variable 是 global 的，在 python 而是 local**

  * **原因是 global variables are generally bad practice and should be avoided**

  * **So when you define variables inside a function definition, they are local to this function by default（python 在 function 內 define variable 的是 local variable）**

  * **應該要跳出題目後**

  * **跳出問題**

  * **輸入一個答案\(for element in list\)**

  * **判斷對與錯**

  * **對就回傳進去**

  * **怎麼取代？讓 part\_of\_speech 內的東西和句子裡一樣就好拉**

  * **猜錯就要再猜**

  * **整段加上猜對的字要顯示出**

  **  
  **

  ### **問題回饋**

  * **No functions are longer than 18 lines of code**

  * **沒有 comment**

  * **應該可以用**

  * **for element in list:, or, to test whether something is in a list,if name in list\_names:\).**

  **  
  **

  ### **目前問題**

  * **輸完答案沒有輸出**

  * **只能輸入一次沒有 loop**

  * **結束不知道**

  **  
  Stage 3 Submit**

  **  
  **

  ### **專案需求**

  **Spec**

  * **要存最喜愛的電影, 資料要包含 URL 和 image**

  * **實作步驟**

  * **Create a data structure \(i.e. a Python Class\) to store your favorite movies, including movie title, box art URL \(or poster URL\) and a YouTube link to the movie trailer.**

  * **Create multiple instances of that Python Class to represent your favorite movies; group all the instances together in a list.**

  * **To help you generate a website that displays these movies, we have provided a Python module called**[**fresh\_tomatoes.py**](https://s3.amazonaws.com/udacity-hosted-downloads/ud036/fresh_tomatoes.py)**- this module has a function called open\_movies\_page that takes in one argument, which is a list of movies and creates an HTML file which visualizes all of your favorite movies.**

  * **Ensure your website renders correctly when you attempt to load it in a browser.**

  **  
  **

  **簡而言之**

  1. **先寫 class，創造 instances**

  2. **用 fresh\_tomatoes.py 內的 open\_movie\_page \( 含argument 和 HTML 視覺\)**

  3. **想一想 class 要有哪些 property，就可以寫 constructor**

  4. **像 movie titles, box art, poster images, and movie trailer URLs**

  5. **在 entertainment\_center.py 用 media.Movie\(\) 創作 objects**

  6. **在 entertainment\_center.py ，calling the constructor media.Movie\(\) to instantiate movie objects**

  7. **在寫個 movies 當作 list ，因為 open\_movies\_page 的 input 要用**

**  
**

* **Mockups**

![](https://lh5.googleusercontent.com/T7BfExX-vaY_dm6mKxXUG2ML22xgCs1VsqKOiVRa-SikaLfZu_HDaKn8AZzKAqgoLz-n__amRWizv5lYBGjtZQvaGkxn0DaTikBudhkRenvw-uGkP6S-HmD46pPfdLY803iGdsY8)

![](https://lh5.googleusercontent.com/31L95azgM_J-AU370or7YSU7ELpkdA9iXh90esLBvDgI7v-aGdLfCQ5eQGEJ200FoWAxuCo1M5RuiGDiiiW9AxBExTj5EugFJVPF63quDS03MtBOouG_8IvdopYqqdIQJRaJBCk7)

**  
**

**  
**

**  
**



  


