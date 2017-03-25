**3.3b Use Classes - Text Send**

**寫 Code 發簡訊**

**Twilio**

* **並非來自 Python Standard Library，是成千上萬的 Python Packages which are available to download to use**

* [**安裝方式**](https://www.udacity.com/course/viewer#!/c-nd000/l-4181149252/m-4750123804)

* **要先成功安裝pip，twilio 才能安裝**

* [**pip**](https://en.wikipedia.org/wiki/Pip_%28package_manager%29)**是什麼？**

* **pip 的**[**Guideline**](https://pip.pypa.io/en/stable/)

* **安裝時輸入的**[**sudo**](http://note.drx.tw/2008/01/linuxsudo.html)**是？**

* [**詳細解說**](https://www.sudo.ws/man/sudo.man.html)

* **要使用**[**sudo - H**](http://stackoverflow.com/questions/28619686/what-is-the-h-flag-for-pip)**的 command line**

* [**Github**](https://github.com/twilio/twilio-python)

* [**解說 Class**](https://www.udacity.com/course/viewer#!/c-nd000/l-4181149252/m-1013498739)**其實就像blueprint 可以創造不同的 object**

* **比較 turtle 和 twilio**

* **turtle 是個 file，內有 Turtle\(\) 和 Screen\(\) 這些 class**

* **rest 是個 folder，est 內的 python 檔案有個class TwilioRentClient，也先call init function，創造記憶體空間**

* **都先跑 init 創造記憶體空間**

**  
**

**關係圖**

**twilio 這個檔案夾下是 rest 檔案夾，rest 內的 python 檔案有個class TwilioRentClient，實際上在 call init function**

![](https://lh5.googleusercontent.com/rZaoTIfdByRT3kbZBxE4cMvrsyVPuFEvXdcFXA23TG-ZFdNm065pVFbHcC_ikwLH1wtG64lC3lkPF85vBsrPb3V7joVMHDn01MAZRhcmD481buL9LIfcuiZulE5W6SVcAoFjHEVF)

**  
**

**from...import**

**let you import specific attributes from a module**

  
**from a file\(module\) name import class**

**send\_sms.py**

* **註冊後到 Dashboard 的 API Credential 查看 SID 和 Token，再套到 Code 裡面**

[**Anaconda**](https://www.continuum.io/downloads)

* **Python 的大補帖，方便把重要套件都一次裝齊全**

* [**學習資源**](https://www.youtube.com/watch?v=WB8hg6UZeY0)

* **Spyder, Anaconda's alternative to IDLE**

**  
**

* **3.3c Use Classes - Profanity Editor**

**案例：檢查文件中有沒有不雅的字眼**

* **使用像 open\(\) &close\(\) 這種內定常用的 built-in function**

* **object 都可以用，不像 Turtle 要 call class**

* [**Built-in function**](https://docs.python.org/2/library/functions.html)

* [**Query String**](https://en.wikipedia.org/wiki/Query_string)

* [**補充資料**](https://www.dotblogs.com.tw/marcus116/2012/07/29/73690)

**流程**

1. **打開檔案**

1. **先用到 open\(\)，打開檔案**

1. **打開的檔案要讀取，用**[**read method**](https://docs.python.org/2/tutorial/inputoutput.html#methods-of-file-objects)**讀檔案**

1. **讀完關掉，close\(\)**

1. **把檔案文字丟到網站**

1. **網站回傳結果**

1. **判斷結果**

**  
**

[**urllib**](https://docs.python.org/2/library/urllib.html)

* **屬於 python standard 原本就有的 module**

* **urlopen 是 function inside**

**  
**

[**為何 urlopen\(\) 和 open\(\) 都沒有要建一個 class?**](https://www.udacity.com/course/viewer#!/c-nd000/l-4212708573/m-1010658699)

**只是表面看不出來，其實 some classes init**

**  
**

* **3.4a Make Classes - Movie Website**

[**Google Python Style Guide**](https://google.github.io/styleguide/pyguide.html)

* **Providing conventions how write python from the world**

* **Google 建議建立新的 class 時，class 的名字第一個字要大寫**

* **e.g. class Movie**

**  
**

[**繼承別的檔案的 Class**](https://www.udacity.com/course/viewer#!/c-nd000/l-4185678656/e-991358854/m-1013629059)

* **在一個檔案創建的 class，可以在別的檔案使用 import 檔名\(不用加py\)**

* **在新檔案創建 object**

* **some module or file name dot a class name**

**e.g. toy\_story = media.Movie\(\)**

![](https://lh6.googleusercontent.com/EfWxpYKqfnVCN6vdZuhT4KuKmZoWG3SN4RqTg8-52YcCGU1VJGq-oJ6Yi7MuKhNxGAR0nl11d53rS1WKOHXrFZ2WB8asIPtDnQg9VTOtBEKFdEXbLUP3AXOJ5yDIp9tVcWMof-jS)

**  
**

**三個觀念**

![](https://lh5.googleusercontent.com/QPJhkk7gNnSOkl_rbOUaeNEuAs9gbNr8kWGYeDViJrawm6kwpxxLZHustzcNOtTn4KHbSABM0r1R02GZV1jWc19pHP92b14mEFMNlShz0UbujcUlOIJOI1G9hN_sPt06VCXkWRQX)**在這邊我們用了新建的檔案1（ media.py ）裏面有個 class Movie，在檔案2寫了 toy\_story = media.Movie\(\)，寫這一行的背後是，call the init function, define inside class movie ; 這個 init 也叫 constructor 因為 constructs space and memory for the new instance**

**  
**

**Defining \_init\_**

* **underscores 告訴 programmers，essentially reserved in Python,this is special method or function**

* **是一種慣例\(convention\)**

* [**詳細解釋**](http://shahriar.svbtle.com/underscores-in-python)

**  
**

**Method 跟 Function 的不同**

[**解釋什麼是 Method**](https://stackoverflow.com/questions/3786881/what-is-a-method-in-python?answertab=votes#tab-top)**， A function which a member of class**

**  
**

**Self**

* **self as itself or the instance being created**

* **self is the object being created**

* [**Udacity 解釋**](https://docs.python.org/2.7/tutorial/classes.html#random-remarks)

* **目前了解就像這個例子裡創造的 object , toy\_story, self 用在你define class 內**

![](https://lh4.googleusercontent.com/IJr_4UO_upqu6Bb60XRH5EK62rc6FKT6xfE2qvuUimipVauBRNssvFPOXii3loUpVBWvutNOhn6uNG24vvFWr8jgVl_CAk2cNWGzFQjZgQsGdEAZOIzRtlYOkVu4OA4uyDBR_oi9)

**你就可以開始利用 self 創造這個 function 下的 property**

**  
**

**instance variables\(e.g. title, storyline...\) 和 instance methods\(e.g. def \_init\_\) 其實就是 define class 時寫的值**

  


