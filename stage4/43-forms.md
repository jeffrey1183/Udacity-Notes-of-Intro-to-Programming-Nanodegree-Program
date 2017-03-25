4.3 Forms

  


Forms are what these users will use to enter text, select from dropdown menus, check checkboxes, etc...

  


![](https://lh3.googleusercontent.com/1y0CrW4r0nWmwApQciyTWiNqLOin8SAo-mTpxWrFY6AQFFUNJ8RDqlbCbVGtVrTRNFKRjxlXhsMD3EcBrTwBva8JRRtI69o4_psSxF4CxfbXLZv8EJvMRzNq9W4SzhVCHE9-UF1W)

* 在加了 input name 後，隨著你輸入的 text 不同，URL 也會變動

![](https://lh5.googleusercontent.com/8wKtja75qkcB0d4Y_FL9KmULaTeWPSombUCFlnCC--ivszkm4dBf1mvKl6IDXhK3PwoZhvjoOnCMq_3J2tYNjD_mFjLDFPuQfRbXIDTIkjObG63aJWHCD_K7G95E74o3eWMFEELT)

* input name="q"

* q is the name of input element

* "q" parameter

* 加入 &lt;input type="submit"&gt;

* 會出現一個 submit 的 button

  


Form Action

* where we want to submit to

* 裡面放 URL, it will send the data there

![](https://lh6.googleusercontent.com/quNLNRmYBku9DyrmBmbcZN2ZRrNcRv4HHAdXfbxjgQYXN6PLW5sTtnQBEHh2n6EuMA61kf4co7ZvtsNBXaZ2irxjMEimYZtC-bqEJ_K0P93KwaX67GzBM6g6p4lGodE3h-O66-nA)

* [案例](https://www.udacity.com/course/viewer#!/c-nd000/l-4190688861/e-48700537/m-48311759),填入 google 後



如果你在框框內輸入 better fiight

* URL 會出現 better+flight

* 因為 URL 裡不能有 space，這時候 URL 其實在做 URL encoding, form encoding or URL escaping

* 結果都是把空格變成 +

* 如果你填入 ! ，他可能跑出[%21](http://www.w3schools.com/tags/ref_urlencode.asp)，就跑掉了

* 可能不同瀏覽器有點不同

  


![](https://lh6.googleusercontent.com/vh4Cz3S6DGGIZH6JttMNHS8lr_DqhvH0oZbTdR5Wpd65ng-3VcH-iFSvSCNKpkS69iBBToR51FFgVrsjJgmfyWLjm7hs8VAQ8SKrY4NVBVwhCUg4lWJFeW9glOUJZUJzz5C9TRp8)

* type ="text" 是 default type of an input parameter

  


![](https://lh3.googleusercontent.com/YeejBA2F4MQ3Ryg_9oh9QO94D0SalyUfZjBwFRoWXlYRCPXLEDAxYhwMw1wocnVpXG1R-l0UDKNzavU4bZBFPsVDKhKdqYJhIhEYQqbFXXYje61vd_GGpArKwNDs9VWZGFs43jjU)

* 開始學習 &lt;input type="password"&gt;

* 還可以換成 checkbox

![](https://lh6.googleusercontent.com/X7SfLPU6KbZhF4aOOjbJ_jH3Dx_qrmlRhP8SWXTNjps4ytOkbUBBedfCgMVxmlSljyyBY6iYK8U0aHcblAShk38k6YA08sqCIofOWeeeEgKFBp8Vxq08kJoiwgNXugGn4BPnT8kG)

* 如果把 name 都換成同樣的 q，就只能一次選一個

![](https://lh5.googleusercontent.com/UihmSfcvn5f1cFcEanfNLK6FhZB18c9G1JroooQ4CZFxxUf2Jtexjb2m8w_GKgCYvi1zwoAdHw872Q7PQoeQnrAs-LvdGOZIUAwKBiLE0-gWsVpAxflskZ5CdVyd7aHAgcM68kKB)

* 加上 value

* 加上 label

```
<label>
one
<input type="radio" name="q" value="one">
</label>
```



Dropdown

```
<form>
<select>
<option>one</option>
<option>two</option>
<option>three</option>
</select>
<input type="submit">
</form>
```

* 一樣可以加上 value

* Google App Engine

* 我的 GAE 連結：[http://axial-willow-118309.appspot.com/](http://axial-willow-118309.appspot.com/)

* [Google Cloud Playground](https://cloud-playground.appspot.com/playground/)

* set up your own server by downloading and installing Google App Engine. This will give you a place to host your web page for free!

* [安裝步驟](https://www.udacity.com/course/viewer#!/c-nd000/l-4166899177/m-3957479131)，創造兩個檔案

* [YAML](https://zh.wikipedia.org/wiki/YAML)格式

* An App Engine application has a configuration file called app.yaml. Among other things, this file describes which handler scripts should be used for which URLs.

* handle requests from the browser and make sure that they are directed to the right place

* 例如要 favicon（網址旁邊的 icon）

* 安裝後選File/Add Existing Application，選擇剛剛建的 Helloworld 資料夾，點 Run 就可以按 Browser

* 你可以修改 helloworld.py 的內容

  


favicon.ico

* [介紹](http://blog.miniasp.com/post/2007/12/17/Introduce-faviconico-and-important-concept.aspx)

  


Regular expression \(Regex\)

* [解說](https://dotblogs.com.tw/johnny/2010/01/25/13301)、[課程](https://www.udacity.com/course/viewer#!/c-nd000/l-4166899177/m-5041309691)

* Regex[念法](https://www.youtube.com/watch?v=EppQdkv4G2w)，都是短音 e

* . \(句點符號\) is a catch-all, which allows us to match any single character

* The \* symbol means the expression will match any number of characters which match the previous symbol.

* So if we have a /.\* , that will allow us to essentially match all strings that come after the last forward slash in the URL and direct them to main.app.

* 有點像轉址

  


* This /.\* is what’s called a regular expression\(Regex\)

* a way of matching strings using symbols.

* 最主要目的, 在於使用一組特定的表示式, 來驗證一段字串是否符合這個樣式 \(Pattern\)

  


  


Creating a Project on Google App Engine

* [教學](https://www.udacity.com/course/viewer#!/c-nd000/l-4166899177/m-3950729245)、[詳解](https://www.udacity.com/course/viewer#!/c-nd000/l-4166899177/m-3905818615)

* 創建後才能 deploy our application 和分享 URL

* 跳到 Uploading the application 的步驟

* 創建你的 project 會有\(Project Name（隨便你叫，個人的） & 唯一的 ID\)

* 如果你要 deploy 你的 application, run it online and share，就把 app.yaml 裡的 application: your-app-id，修改成自己的 google 專案 id （e.g. axial-willow-118309），再 deploy，過程中會顯示訊息

* 最後到 uniqueprojectid.appspot.com

* e.g. axial-willow-118309.appspot.com/

* 常見問題：

* 如果你使用錯誤的 application ID，可能跑出 Error 403,顯示 you don't have permission to modify

* 如果你 yaml 中的 script 打錯了，他抓不到檔案，連結頁面就會有問題

  
Debug 方式 -[看 Log](https://www.udacity.com/course/viewer#!/c-nd000/l-4166899177/m-4991449062)

* 大絕[Troubleshooting Doc](about:blank)

  


* 4.4 Modulus & Dictionaries

Modulus 就是 Modulo 的複數

  


  


The Modulus Operator

* This is an operator \(like +, -, \*, or /\) that every programming language has.

* 為了讓 output 在正確的範圍

* 會用 %，其實就是算餘數

* 3%4，餘數是三唷

![](https://lh4.googleusercontent.com/I1b4ylCCMaPevXsVwAW7mUiIKZzdGpcIbyPW0eJ34hpsBs11iUZFWvr_zvrkp9X6ah63sSxA90To5nuA9k-3rQAtRxkmlrnQOiQoMgL-POrfSMEQMr7s5mtG3wYAn_MACKT94P7E)

  


Dictionaries

* This is another data structure, similar to a Python List.

* 裡面包 Key 和 value

* 前面的 Key，是 immutable\(不可變的\) value

* 不一定是 strings,也可以是 numbers 或其他東西

* value 也不限

* [Hash Table](https://www.youtube.com/watch?v=h2d9b_nEzoA)

  


  


  


[![](https://lh4.googleusercontent.com/IB3qsl3pGTfp7byzNoqfBB-70buT-aTefpjr857TNIlVQ91_u0XxpxP01cuWsj8H2rU-gXV4epSWMuzMavsnLUy3plSHuDh7Sx6BX0t0JMCXdBPXowKOCgkzZgSuWLOYxPCgjgc1)](https://www.youtube.com/watch?v=h2d9b_nEzoA)

List 可放字串和數字，Dictionary 是一個 key 和 value的概念

  


Immutable 和 mutable

* 前者一旦創造就不能改，不變的 value

* String 不能改, List 和 Dictionary 都可以

  


Order - 用 index 找值

* string 和 List 都可以

* Dictionary 中的 d\[K\] 表示你可以用 key 去找你的 value

* 如果用不存在的 key 值去找，會出現 error

* 可以用 in 另外的寫法

* e.g. print 'carbon' in elements

* 會出現 true or flase

* The elements are ordered in list, dictionaries don't

  


改變原本的值

* String 不行

* List 可以，Dictionary 改變 value

  


Dictionaries 增加

  
Use assignment

* 像 elements\['ni'\] = 8

* 也可以修改值 elements\['ni'\] = 9

  


![](https://lh5.googleusercontent.com/Ifx1b2II_-YHKeRbvC0aYeuZhowAkYpxz4iPxGiVf7Z9u89GIQZ4CdpBdNH1MkTtFCz0ewQgvllZaCx0fVPF6gMRVZ-9TvPVIq7awgKa0gTDmK9rJmNYSA7zxkkwx0kRkm_0Skol)

  


Dictionary 可以塞其他 dictionary ， 也可以尋找 key 值

* [影片](https://www.udacity.com/course/viewer#!/c-nd000/l-4181088694/m-48683768)



