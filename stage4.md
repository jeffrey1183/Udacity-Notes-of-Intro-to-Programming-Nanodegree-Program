# **Stage 4**

* **you will set up a server with Google App Engine**

## 解析方程式

```py
def word_in_pos(word, parts_of_speech):
    for pos in parts_of_speech:
        if pos in word:
            return pos
    return None

  # pos 變成 parts_of_speech 的每一個數的代表，如果 pos 有跟
    # word 這個 list 內一樣的 element 就 return 這個 element

def play_game(ml_string, parts_of_speech):
    replaced = []
    ml_string = ml_string.split()
    for word in ml_string:
        replacement = word_in_pos(word, parts_of_speech)
        if  replacement != None:
            user_input = raw_input("Type in a: " + replacement + " ")
            word = word.replace(replacement, user_input)
            replaced.append(word)
        else:
            replaced.append(word)
            replaced = " ".join(replaced)
            return replaced
```

* 這個方程式跟上面那個異曲同工，他把 ml\\_string 加進來比較，目標是把 replaced 的新內容創造出來

* 第三行先把 ml\\_string 拆成字串，一樣用 for ，把這些字串都用 word 去跑，第五行最重要，他其實在比對 parts\\_of\\_speech 的 element 跟 word（拆成 ml\\_string 的個別字串）有沒有一樣的

* 第六行，如果有一樣的話（應該會一樣，早就設好了），第七行開始抓輸入的值，後面 的"Type in a: " + replacement + " "，就是使用者會看到的文案，這裡的 replacement 就是前面對比出有一樣要替代的字串

* 第八行，把 word 中 replacement 用輸入的字替換掉，word 是那些 ml\\_string 分散的字元

* 第九行，list 加上 word 這堆 list

* 第十二行， 把 list 變成字串，可參考 Spit 的相反，join

## 補充：

[raw\\_input](https://www.foolegg.com/how-to-get-the-users-input-in-python-with-input-or-raw_input-functions/)

[stdout](http://bcc16.ncu.edu.tw/6/textutil/03.html)

[append](http://www.tutorialspoint.com/python/list_append.htm) 把 object 加進 list

