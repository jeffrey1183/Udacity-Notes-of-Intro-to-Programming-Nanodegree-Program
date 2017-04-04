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



可以閱讀和編寫基本的 Python 代碼。這門課程會用到 Python 編程練習。如果你之前沒有使用過 Python，請參閱我們的Python：[編程基礎課程。](https://cn.udacity.com/course/programming-foundations-with-python--ud036)

如果你能看懂下面的 Python 代碼（或許需要查閱[random模塊文檔](https://docs.python.org/2/library/random.html#random.choice)），那麼對於本課程來說你的 Python 知識足夠了。

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





你可以使用命令行界面（終端）。本課程中的某些練習題需要使用 Unix 形式的命令行界面來輸入指令，運行 Python 程序和訪問目錄。

如果你已經學習了我們的如何使用 [Git 和 Github課程](https://cn.udacity.com/course/how-to-use-git-and-github--ud775/)，那麼本課程中的命令行使用水平和此課程的比較相似。

**你不需要成為前端開發者。此課程的示例中的確會出現小型網絡應用和一些 HTML，但是你不需要用這些語言做出更改。**

**你不需要具備任何數據庫經驗。這門課程是關系數據庫的入門級介紹。**



