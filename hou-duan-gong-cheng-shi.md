這門課程非常有趣，會使用 Python 示例快速介紹如何在代碼中使用關係數據庫。你將學習結構化查詢語言 \(SQL\) 基礎知識和數據庫設計，以及將 Python 代碼與數據庫相關聯的 Python API。你還將稍加學習如何保護你的數據庫後端網絡應用，讓它不受常見安全問題的侵擾。

如果你查看了各種大型網站（從維基百科到 Reddit）的源代碼，就會發現網站某個地方使用了關係數據庫。多年來，數據庫系統（例如 PostgreSQL 和 MySQL）一直是開發者常用的工具，繼續成為存儲和操作結構化數據最強大的工具。

如果你打算繼續在全端開發領域發展，了解數據庫則是必備的背景要求。即使很多工具包以及針對你的應用代碼隱藏了數據庫詳情，能夠與數據庫互動將非常有助於設計、調試和操控應用。

# 學習計劃

---

## 第 1 課：數據和表格

在這節課中，你將學習如何使用關系數據庫將數據變成表格。你將學習唯一鍵的重要性和表格之間的關系。

## 第 2 課：SQL 元素

在這節課裡，你將開始學習大多數關系數據庫用到的結構化查詢語言 \(SQL\)。你將學習選擇和插入語句，二者是從數據庫中獲取數據和向數據庫中插入數據的基本操作。你將學習瀏覽表格和整合表格的運算符及語法。

## 第 3 課：Python DB-API

在這節課裡，你將學習如何使用 Python 代碼訪問關系數據庫。你將使用在你自己的計算機上運行的虛擬機運行 Python 網絡應用，並使該應用使用數據庫後端。然後，你將學習數據庫應用會出現的一些最常見安全風險，包括著名的 [Bobby Tables](https://xkcd.com/327/)。這節課還會介紹 SQL 更新和刪除語句。

## 第 4 課：深入學習 SQL

在這節課裡，你將學習如何設計和創建新的數據庫。你將學習正態化設計，這樣可以更輕松地使用數據庫編寫有效代碼。你還將學習如何使用 SQL 連接運算符快速連接不同表格中的數據。

## 第 5 課：最終項目

在此項目中，你將運用所學的 Python 和 SQL 知識構建一個基於數據庫的 Python 應用來運行競標賽。你將設計數據庫架構並編寫代碼來實現此項目的 API。

## 先修要求 {#-}

**你可以阅读和编写基本的 Python 代码。**这门课程会用到 Python 编程练习。如果你之前没有使用过 Python，请参阅我们的[Python：编程基础](https://cn.udacity.com/course/programming-foundations-with-python--ud036)课程。

如果你能看懂下面的 Python 代码（或许需要查阅[**random**模块文档](https://docs.python.org/2/library/random.html#random.choice)），那么对于本课程来说你的 Python 知识足够了。

```python
import random

def ChooseTwice(items):
    a = random.choice(items)
    b = random.choice(items)
    return a, b

names = ["Alice", "Bob", "Charlie", "Debra"]
(one, two) = ChooseTwice(names)
if one == two:
    print "%s is happy!" % one
else:
    print "%s likes %s!" % (one, two)
```

**你可以使用命令行界面（终端）。**本课程中的某些练习题需要使用 Unix 形式的命令行界面来输入指令，运行 Python 程序和访问目录。

如果你已经学习了我们的[如何使用 Git 和 Github](https://cn.udacity.com/course/how-to-use-git-and-github--ud775/)课程，那么本课程中的命令行使用水平和此课程的比较相似。

**你不需要成为前端开发者。**此课程的示例中的确会出现小型网络应用和一些 HTML，但是你不需要用这些语言做出更改。

**你不需要具备任何数据库经验。**这门课程是关系数据库的入门级介绍。

**你需要在计算机上安装一个编程文本编辑器**（例如[Sublime Text](http://www.sublimetext.com/)）。你应该能够使用该编辑器打开和编辑 Python 代码文件。

